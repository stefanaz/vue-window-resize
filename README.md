# vue-window-resize

## Description
A very simple vue component to have a window width and height reactive values on window resize. 

## Install and basic usage:

```sh
npm install --save vue-window-resize@latest
```

### Usage:
Window variable is reactive and shows actual width/height on window resize. 
```js
    <VueWindowResize v-show="false" v-model="window"/>
    ...
    export default {
        data() {
          return {
                window: {
                    width: 0,
                    height: 0
                },
            }
        }
        // rest of the component
    }
    ...
```


### Register the component globally
```js
import Vue from 'vue'
import VueWindowResize from 'vue-window-resize'
Vue.component('VueWindowResize', VueWindowResize)
```

### Register the component locally
```js
import VueWindowResize from 'vue-window-resize';

export default {
  components: {
    VueWindowResize,
  },
  // rest of the component
}
```

### Register via **\<script>** tag 
```js
<script src="https://unpkg.com/vue-window-resize@1.0.4/dist/vue-window-resize.umd.min.js"></script>

...
<vue-window-resize v-model="window"></vue-window-resize>
...
```


