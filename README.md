# react-native-casino-roulette

### Whats new in this fork?

Added `spin(direction)` function
direction parameter can be set to `counterClockwise` for counter clockwise spin or be set to anything else for clockwise

![](https://cdn.rawgit.com/DKbyo/react-native-roulette-casino-demo/711e0cc2/demo.gif)

### Installation
```bash
npm install react-native-casino-roulette
```

### Properties

```
options // Array of choices

step // Roulette items margin
radius = {300} // Roulette radius
distance = {100} // Distance from center
rouletteRotate = {0} // Roulette rotate angle
enableUserRotate = {false} // Enable user input for rotate
background = {require('./background.png')} // Set background image
marker = {require('./marker.png')} // Set marker image
markerWidth = {require('./marker.png')} // Set marker width
markerTop: 0, // Marker top position
onRotate = () => {} // Return active option after rotation
onRotateChange = () => {} // Return rotate change status
rotateEachElement = () => 0 // Return rotate angle for each element
options= {[1,2,3]} // Set array of options
customStyle // Roulette styles
centerImage: null, // Center image (This image will not spin)
centerTop: 0, //Center width position
centerWidth:20, // Center width
markerStyle: {} // Custom marker style
```

### Quick example
```
...

import Roulette from 'react-native-roulette';

//Roulette numbers
const numbers = [0,32,15,19,4,21,2,25,17,34,6,27,13,36,11,30,8,23,10,5,24,16,33,1,20,14,31,9,22,18,29,7,28,12,35,3,26]
const options  = numbers.map((o)=>({index:o}))  

<Roulette 
          enableUserRotate 
          background={wheel}
          marker={marker}
          options={options}
          markerWidth={20} >          
</Roulette>
...

```

### Full example

For full example see [here](https://github.com/DKbyo/react-native-roulette-casino-demo)


