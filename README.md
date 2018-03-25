# VueNumberFormating
vue convert number to decimal formating

# install

```javascript
> npm install --save vue-number-formating
```

## config
 1 ) create file plugin/VueNumberFormating.js 

```
 import Vue from 'vue'
 import VueNumberFormating from 'vue-number-formating'

 Vue.use(VueNumberFormating);
 
```

2 ) import To main.js

```
    import Vue from 'vue'
    import App from './App.vue'
    import VueNumberFormating from './plugin/VueNumberFormating'
        
    new Vue({
      el: '#app',
      render: h => h(App),
    }); 
```


## use
````
    <template>
        <p>{{ $nF.numberToFormat(1500000) }}</p>
        <span> Convert In 1,500,000 </span>
    </template>
    
    // OR
    
    <script>
        export default {
            mounted() {
                this.$nF.numberToFormat(1500000); // conevrt to 1,500,000
            }
        }
    </script>
    
````



