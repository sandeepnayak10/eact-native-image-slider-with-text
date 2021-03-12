
# react-native-image-slider-with-text

## Install

1. First, install our library | use below npm script

   > npm i react-native-image-slider-with-text

   > yarn add react-native-image-slider-with-text
Well-done.

## Usage :

### list of available props for customization SliderBox:

| Props                        | Value Type                            | Description                                                                                                                                             |
| ---------------------------- | ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ImageComponent`             | Image component, default as `Image`   | default value is React-native Image, if you use third-party library like FastImage use this property                                                    |
| images                       | Array of image path(or url) as string | Set array of images path- these paths can contain `http url link` or `local images path` using `require('./pathOfImage')`                                                                    |
| onCurrentImagePressed        | handler function callback             | callback for get pressed image index (index start from 0)                                                                                               |
| currentImageEmitter          | handler function callback             | callback for get current image index (index start from 0)                                                                                               |
| disableOnPress               | boolean               |               if present, then onCurrentImagePressed will be disabled                            |
| sliderBoxHeight              | int value                             | default value = 200, you can change height of image slider box                                                                                          |
| parentWidth                  | int                                   | default = screen.width ; in advance mode, if parent is smaller, you can change it. best practice is use onLayout handler in parent component or screen. |
| dotColor                     | color string code                     | change color of paging dot                                                                                                                              |
| inactiveDotColor             | color string code                     | change color of inactive paging dot                                                                                                                     |
| dotStyle                     | style object                          | default style is : {width: 10,height: 10,borderRadius: 5,marginHorizontal: 0,padding: 0,margin: 0,} change style of paging dots if you want            |
| paginationBoxVerticalPadding | int value                             | default = 10 ; change the height of paging dots from bottom of Slider-Box                                                                               |
| autoplay                     | bool value                            | default = false                                                                               |
| circleLoop                   | boolean - attribute                   | if set, when user swiped to last image circularly return to the first image again.                                                                      |
| paginationBoxStyle           | object,default values use lib style   | customize pagination box                                                                                                                                |
| dotStyle                     | object,default use lib style          | customize dot styles                                                                                                                                    |
| resizeMethod                 | string                                | default is `resize`                                                                                                                                     |
| resizeMode                   | string                                | default is `cover`                                                                                                                                      |
| ImageComponentStyle          | object                                | {} style object for ImageComponent   |
  | imageLoadingColor            | string                                | default is `#E91E63` , image loading indicator color       |
| ImageLoader            | React component, default as `ActivityIndicator`                                | default value is React-native ActivityIndicator.
       |
| firstItem            | number                                | default is 0 , index of image to display when slider box loads       |

## Notice:

This library use `react-native-snap-carousel` and make easier way to create image slider box with full customization ability.

See original Library [https://github.com/archriss/react-native-snap-carousel](https://github.com/archriss/react-native-snap-carousel)

we dont edit or modify original library, we just use it with some additional style. (BSD 3 License)
