<template>
  <div>
    <span>Server #{{ id }} - {{ status }}</span>
    <button class="btn btn-primary" @click="changeStatus">Change Status</button>
  </div>
</template>

<script>
  export default {
    data: function() {
      return {
        id: 0,
        status: 'Normal'
      }
    },
    methods: {
      changeStatus() {
        this.status = 'Critical';
      }
    }
  }
</script>

<style>

</style>

