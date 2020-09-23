<template>
  <div class="home">
    <h1>counter: {{counter}}</h1>
    <button @click="increCounter">incre</button>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'Home',
  setup() {
    const counter = ref(1);
    function increCounter() {
      counter.value++;
    }
    return {counter, increCounter}
  },
  components: {
  },
});

</script>
