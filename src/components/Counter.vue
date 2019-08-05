<template>
  <div class="counter">
    <h1>Counter</h1>
    <p>
    </p>
    <p>
      <button @click="decrement">-</button>
      <span>{{count}}</span>
      <button @click="increment">+</button>
    </p>
  </div>
</template>

<script>
export default {
  name: 'Counter',
  data() {
    return { count: 0 };
  },
  methods: {
    increment() {
      this.count += 1;  
    },
    decrement() {
      this.count -= 1;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  margin: 0 20px;
}
</style>
