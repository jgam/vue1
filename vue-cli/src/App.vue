<template>
  <div>
    <app-header v-on:renew="onRenew" v-bind:header="str"></app-header>
    {{str}}
  </div>
</template>

<script>
import AppHeader from './components/AppHeader';
export default {
  data: function(){
    return {
      str: 'Headerrr'
    }
  },
  components:{
    'app-header':AppHeader
  },
  methods:{
    onRenew: function(){
      this.str = 'hi'
    }
  }
}
</script>

<style>

</style>