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

  setup() {
        const navLinks = ([{
                name: "Home",
                path: "/",
            },
            {
                name: "About",
                path: "/about",
            },
            {
                name: "FAQs",
                path: "/faqs",
            },
            {
                name: "More",
                path: "/more",
            },
            {
                name: "Media",
                path: "/media",
            },
        ]);

        const navConfig = ({
            
            navBg: "#000",
            linkFont: "Sans-serif",
            linkColor: "#fff",
            linkColorHover: "#fff",
            navLogo: "https://interactive-examples.mdn.mozilla.net/media/cc0-images/grapefruit-slice-332-332.jpg",
        });

        return {
            navLinks, navConfig
        };
    },
```


```xml
<template>
  <VueNavbarResponsive :navLinks="navLinks" :navConfig="navConfig"/>
</template>
```



