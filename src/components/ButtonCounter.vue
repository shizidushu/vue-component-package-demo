<template>
  <button v-on:click="count++">你已点击 {{ count }} 次.</button>
</template>

<script>
export default {
  name: 'button-counter',
  data: function() {
    return {
      count: 0
    };
  }
};
</script>
