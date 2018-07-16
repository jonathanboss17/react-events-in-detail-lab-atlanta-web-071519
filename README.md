# React Events in Detail

## Overview

In this lab, you'll work with event data and persisting events.

## Two Buttons To Rule Them All

![Using buttons](https://media.giphy.com/media/HraQGUYyPxDz2/giphy.gif)

In this lab, you'll be working on two components — two buttons, to be more
precise. These aren't just regular buttons, however! They both serve a very
specific purpose.

#### `CoordinatesButton`

1. In the `components/CoordinatesButton.js` file, create a `CoordinatesButton` React component.

2. This component takes in one prop: `onReceiveCoordinates`. This prop is a
_function_ passed down from `index.js`. This function is currently just logging
whatever is passed into it.

3. Within `CoordinatesButton`, render a button. On click of the button,
create an array with two elements: the X and Y coordinates of the mouse. Find
these using the event data.

4. Pass this event data in as the argument for the `onReceiveCoordinates` prop.

5. If successful, the current x,y position of your mouse should be logged.

#### `DelayedButton`

1. In the `components/DelayedButton.js` file, create a `DelayedButton` React component

2. This component takes two props: `onDelayedClick` (a function), and `delay` (a
number).

3. Create a button that, when clicked, will pass the click event to the
`onDelayedClick` prop _within_ a `setTimeout()`. The `setTimeout()`
should be set to `this.props.delay`.

4. If successful, the event will be logged to the console once the timeout has finished.

## Resources

- [React Mouse Events](https://facebook.github.io/react/docs/events.html#mouse-events)
