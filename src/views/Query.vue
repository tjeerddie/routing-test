<template>
  <div class="home">
    <HelloWorld msg="Other"/>
    <pre>{{ $route.query }}</pre>
    <button @click="log">button</button>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'other',
  components: {
    HelloWorld,
  },
  methods: {
    log() {
      console.log(this.$route);
    },
  },
};
</script>
