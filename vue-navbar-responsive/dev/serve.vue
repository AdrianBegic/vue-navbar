<script>
import { defineComponent } from 'vue';
import VueNavbarResponsive from '@/vue-navbar-responsive.vue';

export default defineComponent({
  name: 'ServeDev',
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
});
</script>

<template>
  <div id="app">
    <vue-navbar-responsive :style="header" />
  </div>
</template>
