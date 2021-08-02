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
| Parameter | Required | Type                       | Default         | Description                                                                                                                                                            |
|-----------|----------|----------------------------|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| type      |          | String                     | 'fade-in'       | Animation type. Available animations: 'fade-in', 'slide-in', 'custom'. If type is 'custom' you have to set initialState and finalState as an object of css properties. |
| offset    |          | Number                     | 0.5             | Intersection observer offset                                                                                                                                           |
| target    |          | DOM Node \|\| CSS Selector | current element | Target of animation                                                                                                                                                    |
| duration  |          | Number                     | 1.2             | Duration of animation                                                                                                                                                  |
| ease      |          | String                     | 'expo.out'      | Type of ease. Based on GSAP Eases documentation > https://greensock.com/docs/v3/Eases                                                                                  |

