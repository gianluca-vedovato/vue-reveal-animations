# vue-accordion
Vue directive for reveal animations based on Intersection Observer.
## Installation
```
npm i vue-reveal-animations
```
or
```
yarn add npm i vue-reveal-animations
```

Then you can install your plugin globally with
```
...
import revealAnimations from 'vue-reveal-animations'

Vue.directive('reveal-animations', revealAnimations)
...
```
or locally
```
...
import revealAnimations from 'vue-reveal-animations'

export default {
  ...
  directives: {
    revealAnimations
  },
  ...
}
...
```
## Usage
Use as directive with object props as bind.
```
<div v-reveal-animations="options">
  ...
</div>
```

## Options
| Parameter    | Required | Type            | Default                                        | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|--------------|----------|-----------------|------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| type          |      | String          |    'fade-in'                                            | Animation type. Available animations: 'fade-in', 'slide-in', 'custom'. If type is 'custom' you have to set initialState and finalState as an object of css properties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| offset          |          | Number          |           0.5     |                               | Intersection observer offset                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

| target          |          | DOMNode or CSS Selector          |           current el    |                                | Target of animation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| duration          |          | Number          |           1.2         |                           | Animation duration                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ease          |          | String          |           'expo.out'       |                             | Ease value based on GSAP Documentation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |




