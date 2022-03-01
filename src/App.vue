<template>
<Nav :navLinks="navLinks" :navConfig="navConfig"/>
</template>

<script>
import Nav from "./components/nav.vue";

export default {
    name: "App",
    components: {
        Nav,
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

    
};
</script>

<style>
* {
    margin: 0;
    padding: 0;
}
</style>
