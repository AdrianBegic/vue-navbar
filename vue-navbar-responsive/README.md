# vue-navbar

Simple Vue.js Responsive Navbar component.



## Features

- Simple
- Responsive
- Can Be Styled  




## How to use


In the shell:            

```
npm i vue-navbar-responsive
```
In your component file:
```vue



import VueNavbarResponsive from 'vue-navbar-responsive';

export default {
  name: 'App',
  components: {
  VueNavbarResponsive
  },

  data() {
    return {
      header: {
        color: "#222",
        fontSize: "1em",
        backgroundColor: "#666",
        padding: "10px",
      },
    };
  },
```


```xml
<template>
  <VueNavbarResponsive :style="header" />
</template>
```



