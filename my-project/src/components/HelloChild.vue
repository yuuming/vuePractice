<template>
 <div>
  <p>{{title}}</p>
  <p>{{message}}</p>
 </div>
</template>
 
<script>
export default {
  data: function () {
    return {
      title: 'Hello Child vue'
    }
  },
  props: ['message']
}
</script>
