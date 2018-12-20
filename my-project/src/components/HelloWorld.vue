<template>
 <div>
  <p>{{title}}</p>
  <hello-child message= Hello Child vue/>
 </div>
</template>
 
<script>
import HelloChild from './HelloChild'
export default {
  data: function () {
    return {
      title: 'Hello world'
    }
  },
  components: {
    HelloChild
  }
}
</script>