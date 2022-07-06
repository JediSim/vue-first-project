<template>
  <div>bonjour</div>
  <p>{{ count }}</p>
  <button @click="increment">Increment</button>
  <button @click="decrement">decrement</button>
</template>

<script>
export default {
  name: "CounterItem",
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
  },
  mounted() {
    console.log("mounted");
  },
};
</script>
