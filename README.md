# react-hook-screen-orientation :arrows_clockwise:

A React hook for detecting [screen orientation](https://developer.mozilla.org/en-US/docs/Web/API/Screen/orientation).

## Installation

Using `npm`:

```sh
npm install --save react-hook-screen-orientation
```

Using `yarn`:

```sh
yarn add react-hook-screen-orientation
```

## Usage

```jsx
import React from 'react'
import screenOrientation from 'react-hook-screen-orientation'

const ComponentWithScreenOrientation = () => {
  const screenOrientation = useScreenOrientation()

  return (
    <p>Screen orientation is: {screenOrientation}</p>
  )
}
```

## Notes

The `screenOrientation` value provided by the hook is the `type` propery of a [`ScreenOrientation` interface](https://developer.mozilla.org/en-US/docs/Web/API/ScreenOrientation/type) is always one of the following strings:
- `portrait-primary`
- `portrait-secondary` (meaning upside down)
- `landscape-primary`
- `landscape-secondary` (meaning upside down)

## Contributions

Contributions are welcome. File bug reports, create pull requests, feel free to reach out at tothab@gmail.com.

## Licence

LGPL-3.0
