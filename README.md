[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# image-auto-scroll

A simple React Native component that implements Auto Scrolling Image Carousel.

- You can use that for displaying ads.

## Installation

If using yarn:

```
yarn add image-auto-scroll
```

If using npm:

```
npm i image-auto-scroll
```

## Usage

```
import { ImageCarousel } from 'image-auto-scroll';
```

Simply place a `<BackgroundCarousel />` .

```
<View style={{flex:1}}>
    <BackgroundCarousel images={images} time={2000} />
</View>
```

- Pass an array of images into images.
- Pass the time in ms into the time after which the image will change automatically.

## Example

```

import React from "react";
import { StyleSheet, View } from "react-native";
import { ImageCarousel } from "image-auto-scroll";

const images = [
 "https://images.unsplash.com/photo-1508138221679-760a23a2285b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60",
 "https://images.unsplash.com/photo-1485550409059-9afb054cada4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=701&q=80",
 "https://images.unsplash.com/photo-1519125323398-675f0ddb6308?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80",
 "https://images.unsplash.com/photo-1429087969512-1e85aab2683d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80",
 "https://images.unsplash.com/photo-1505678261036-a3fcc5e884ee?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80"
];

export default function App() {
 return (
   <View style={styles.container}>
     <BackgroundCarousel images={images} time={2000} />
   </View>
 );
}

const styles = StyleSheet.create({
 container: {
   flex: 1,
   backgroundColor: "#fff",
   alignItems: "center",
   justifyContent: "center"
 }
});


```
