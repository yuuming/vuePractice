<template>
 <div>
  <p>{{title}}</p>
  <!-- <p><input v-model="input_msg"></p> -->
<p>{{ total }}</p>
  <!-- <hello-child :message="input_msg" /> -->
  <hello-child v-on:increment="incrementTotal" />
 </div>
</template>
 
<script>
import HelloChild from './HelloChild'
export default {
  data: function () {
    return {
      title: 'Hello world',
      total: 0
    }
  },
  methods: {
    incrementTotal: function() {
      this.total += 1
    }
  },
  components: {
    HelloChild
  }
}
</script>