<template>
  <div class="home">
    <HelloWorld msg="Other"/>
    <button @click="log">button</button>
    <pre>{{ $route.query }}</pre>
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
