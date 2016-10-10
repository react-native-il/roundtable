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

