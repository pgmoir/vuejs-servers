<template>
  <div class="cols-xs-12 col-sm-6">
    <ul class="list-group">
      <li class="list-group-item" v-for="index in 5" :key="index.id">
        <app-server :id="index.id"></app-server>
      </li>
    </ul>
  </div>
</template>

<script>
  import Server from './Server'

  export default {
    components: {
      'app-server': Server
    }
  }
</script>

<style scoped>
  div {
    border: 1px solid red;
  }
</style>


