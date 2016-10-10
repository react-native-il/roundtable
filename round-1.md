# Round 1

Meeting at Klarna.
Thanks for everyone for the discussion, it was fantastic! our first round in the roundtable!


## Discussion

### Intro

Format - we gather every once in a while, around a table, where each person
has some React Native experience, or a strong agenda surrounding React Native.

We bring up topics together in an unconference style, and choose which ones to
discuss. At the trivial case, people will present problems, and other people will
present how they solved it, and perhaps other people will even improve on that.

At the more complicated case, if a shared interest exists - the problem can be
solved by a group of otherwise unrelated people.

The surrounding motto is a smaller, tighter, more intimate forum that allows
for disussing intermediate to advanced topics for engineering or management
(i.e. decision making); in a shared way for the benefit of everyone.

We'll present meeting notes here, in the style of the [core react
notes](https://github.com/reactjs/core-notes)


### Why are we here

We gathered the following insights, collaboratively. The basic question
was - why are we all here, taking the effort to meet?

For React Native:

- Lowering the surprise factor
- Model the friction between Web / Native development.
- Production best practices (crashes, logging, analytics)
- Native
- React Native
- Solving the paradox of options (ecosystem)
- How do we decide?
- State management (mobx, redux, flux)
- Training (emph. native)
- Workflow
- Tooling
- Builds, CI, etc.
- Web + Native shared codebase?
- Shared codebase architecture
- Flexbox

### What's percieved as hard in native development?

For this question, the following popped up:

- Testing
- Fragmentation (Android, iPhone 7s)
- UI
- Visuals
- Interactions / Animation
- Tooling
- XCode, Android Studio

### How about Javascript?

- Picking the right flavor (language)
- Typing: flow/TS
- Performance

### Topics we discussed

- Workflow
- Dead ends, sharp ends: sourcemaps, Android maturity, Android keyboard tracking, modifiying core react native problematic - _a solution discussed_
- Crashes, logging: source maps - _Sentry recommended_
- Redux, Mobx - discussion - _towards the end, a quick Mobx demo_

refs:
- [fs walker](https://github.com/jondot/react-native-fs-walker)
- React native inlining: react-packager/src/JSTransformer/worker/inline.js

### ExponentJS
Watch the 2 minute video on [Exponent](https://getexponent.com/) homepage to get a basic understanding of what it is.

They have some nice packages too and not all of them require Exponent to work. I was using [ex-navigation](https://github.com/exponentjs/ex-navigation) before I switched over to Exponent.

What I think is really cool about Exponent and why I'd recommend using it is:

* You can run your apps on *any* device real device in an instance without connecting any wires. To do this the phone just has to have the Exponent app installed on it which is available for both iOS and Android. Once installed, you can demo the app on the phone within 30 seconds and update in second just like you would when developing locally.

* Exponent makes it really easy to add more complex features. For my own app I had a big headache adding Facebook/Google login, eventually got it working and then somehow managed to break it again. With Exponent it worked in minutes. The documentation is basically one paragraph: https://docs.getexponent.com/versions/v10.0.0/sdk/facebook.html. If you try to add Facebook the usual way you'll have to follow multiple sets of instructions, and will have to change things in both XCode and Android studio to get it working. With Exponent it just works. I haven't tried Maps, Push notifications and other Exponent integrations, but they're also supposed to be easy to use straight out the box.

* Exponent has a build tool that will allow you to generate the `.apk` or `.ipa` file in minutes. Just run: `exp start` followed by `exp build:android` or `exp build:ios`. They say it has been heavily tested for Android, but not for iOS, so beware. I haven't had any problems with it myself, but I'm only half way through the submission process. I'm waiting for Apple and Google to approve Beta versions of my app. The `.apk` worked fine on my own Android phone. You can read more about building standalone apps with Exponent [here](https://docs.getexponent.com/versions/v10.0.0/guides/building-standalone-apps.html).

* They have a great team of friendly people and an active [Slack channel](https://slack.exponentjs.com/) which is very helpful.

#### Things to watch out for with Exponent
The biggest drawback to using Exponent is no native modules. From the docs:

> The most limiting thing about Exponent is that you can't add in your own native modules... Right now, Exponent doesn't support custom native code, including third-party libraries which require custom native components. In an Exponent project, you never write native code--only pure JS.

> In our SDK, we give you a large set of commonly desired, high-quality native modules. However, if you need something very custom--like on-the-fly video processing or low level control over the Bluetooth radio to do a firmware update--then Exponent won't work for you and you should instead use regular React Native.

This has effected my own project by not allowing me to add Google login at this moment in time. This is something the Exponent team hopes to add in the next 6 weeks (when Exponent v12 comes out. We're on v10 at the moment.)

One other thing to take note of is that Exponent uses a fork of React Native, so it's not always on the last version of RN. At the time of writing, React Native is on 0.34 and the Exponent fork is at 0.33. They try to be within one month of RN major releases if I rememember correctly.

### List of topics (for next time)

- Workflow
- Dead ends, sharp ends
- Crashes, logging
- Performance
- Routing
- Redux / State management
- Async
- Training and working as a 3-headed beast
- How much native is in native?
- Misunderstandings
- Testing
- Device, e2e testing

