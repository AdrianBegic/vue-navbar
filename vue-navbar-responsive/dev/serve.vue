<script>
import { defineComponent } from 'vue';
import VueNavbarResponsive from '@/vue-navbar-responsive.vue';

export default defineComponent({
  name: 'ServeDev',
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
            navLogo: "https://interactive-examples.mdn.mozilla.net/media/cc0-images/grapefruit-slice-332-332.jpg",
        });

        return {
            navLinks, navConfig
        };
    },
});
</script>

<template>
  <div id="app">
    <vue-navbar-responsive :navLinks="navLinks" :navConfig="navConfig"/>
  </div>
</template>
