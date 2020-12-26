<template>

  <header>
      <h1>{{header}}</h1>
      <button v-on:click="onClick"></button>
  </header>
</template>

<script>
export default {
    methods:{
        onClick: function(){
            console.log('clicked')
            this.$emit('renew');
        }
    },
    props:{
        header: String
    }
}
</script>

<style>

</style>