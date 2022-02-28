<template>
<Nav :style="options"/>
</template>

<script>
import Nav from './components/nav.vue'

export default {
    name: 'App',
    components: {
        Nav,
    },

    data() {
        return {
          options: {

            header: {
                color: '#222',
                fontSize: "1em",
                backgroundColor: '#666',
                padding: '10px'
            },
          },
        }
    },

}
</script>

<style>
* {
    margin: 0;
    padding: 0;
}
</style>
