<template>
  <div>
    <button v-bind:class="classObject">
    "v-on:click="counter += 1">{{label}}</button>
    <h1>{{ CsButton }} </h1>
  </div>
</template>

<script>
export default {
  name: "CsButton",
   props: {
    label: String,
  },
  data: function () {
    return {
      counter: 0,
      classObject:{
          active:true,
          'text-danger':false,
          weight:20,
      },
    }
  },
};
</script>

<style>
</style>