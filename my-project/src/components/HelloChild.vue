<template>
 <div>
  <p>{{title}}</p>
  <button v-on:click="incrementCounter">{{ counter }}</button>
  <!-- <p>{{message}}</p> -->
 </div>
</template>
 
<script>
export default {
  data: function () {
    return {
      title: 'Hello Child vue',
      counter: 0
    }
  },
  methods: {
      incrementCounter: function () {
    this.counter += 1
    this.$emit('increment')         
      }
  }
}
</script>
