# VueNumberFormating
vue convert number to decimal formating

# install

```javascript
> npm install --save vue-number-formating
```

```javascript
> yarn add vue-number-formating
```

## config
 1 ) create file plugin/VueNumberFormating.js 

```javascript
 import Vue from 'vue'
 import VueNumberFormating from 'vue-number-formating'

 Vue.use(VueNumberFormating);
 
```

2 ) import To main.js

```javascript
    import Vue from 'vue'
    import App from './App.vue'
    import './plugin/VueNumberFormating'
        
    new Vue({
      el: '#app',
      render: h => h(App),
    }); 
```


## use
````javascript
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

remove comma : 

```javascript
this.$nF.removeCommasAmount('1,500,000'); // conevrt to 1500000
```





