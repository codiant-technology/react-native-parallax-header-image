# Parallax header with image animation
     
  <p align="center">
   <img  width="300" height="450"  src="/Screenshot_1613741272.png">
  </p>
  ## React Native Hyper Pay (Only for Android)
  
  It provides a parallax header view with an input and elegant image animation.
  
### Installation

`$ react-native-parallax-header-image`

Or

`$ react-native-parallax-header-image`

### Example

```js
import React from "react";
import ParallaxHeader from "react-native-parallax-header-image";
import List from "./List"; // your list component

const ParallaxHeaderDemo = () => {
  return (
    <ParallaxHeader
      headerImage={{
        uri:
          "https://image.shutterstock.com/image-photo/white-transparent-leaf-on-mirror-260nw-1029171697.jpg",
      }}
      leftImage={{
        uri:
          "https://interactive-examples.mdn.mozilla.net/media/cc0-images/grapefruit-slice-332-332.jpg",
      }}
      renderHeader={() => {
        return <Text>{`Hello`}</Text>;
      }}
    >
      <List />
    </ParallaxHeader>
  );
};

export default ParallaxHeaderDemo;
```

### install dev dependencies:

```sh
npm i react-native-parallax-header-image @storybook/addon-knobs faker 
```

| Prop               | Description                                    | Default            |
| ------------------ | ---------------------------------------------- | ------------------ |
| **`headerImage`**  | Valid image source of local or network `image` | defaultHeaderImage |
| **`leftImage`**    | Valid image source of local or network `image` | defaultLeftImage   |
| **`renderHeader`** | Any React Component                            | defaultHeader      |

<!-- | **`headerImageHeight`** | Height of header Image `type: number`          | `100`              |
| **`headerImageWidth`**  | Width of header Image `type: number`           | `200`              | -->

<!-- | **`onPress`**         | A function called when the button is pressed.                                                                                                     | _None_              | -->
