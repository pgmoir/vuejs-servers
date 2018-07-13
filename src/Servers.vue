<template>
  <div>
    <div class="row">
      <div class="cols-xs-12 col-sm-6">
        <ul class="list-group">
          <li class="list-group-item" v-for="index in 5" :key="index.id">
            <app-server :id="index.id"></app-server>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6">
        <p>Server Details are currently not updated</p>
      </div>
    </div>
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

<style>

</style>

