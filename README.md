# React Native Chat UI Example
A barebones example of a texting-style chat interface

![Chat Demo GIF](https://github.com/llamaluvr/ChatUIExample/blob/master/ChatUIDemo.gif "Chat Demo GIF")

## Goal
There's already a handful of fine tutorials on creating a React Native chat app. Heck, you should probably avoid creating your own chat interface and stick with [Gifted Chat](https://github.com/FaridSafi/react-native-gifted-chat "Gifted Chat"). Anyway, for the adventurous folks who do want to create their own chat UI, what I didn't see were any barebones examples/ tutorials that only demonstrated the mechanics of the user interface (and didn't dive into hooking up actual data) and were simple enough to be quick to explain yet competent enough to handle all of the weird cases that you would think about within the first half hour of setting out to make a chat UI.

## What it does
- Shows (lightly) stylized left and right message bubbles
- Moves the bottom input bar up and down with the keyboard
- Moves the last message along with the keyboard (so you're seeing the last message when you go to type)
- Expands the textbox in the input bar to fit the size of the text, and adjusts the ScrollView above so the last message isn't hidden

## What it doesn't do
- Not look a little choppy when sending a message that expands the input bar (no option to animate reset of AutogrowInput back to default size. The fundamentals of this control are good, but it could be forked to add options).
- Perform especially well. There's plenty of room for tightening things up.
- I've heard some of these things can be fiddly on Android. Maybe they're not anymore. Anyway, I didn't test this yet on Android, only the iOS simulator.

## How do I try it?

Typical React Native stuff:
1. [Install React Native](https://facebook.github.io/react-native/docs/getting-started.html)
2. Go to the directory where you downloaded this
3. Run `react-native run-ios`

## Where's the magic?

99.99% of interesting code is in ChatView.js.
