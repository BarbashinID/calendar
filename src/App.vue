<template>
<button v-on:click="localeRu">
    Ru
</button>
<button v-on:click="localeEng">
    Eng
</button>
  <div>Calendar</div>
  <VDatePicker  v-bind:locale = language v-model="date" mode="dateTime" is-required/>
</template>

<script>
export default {
  data(){
    return {
      language: 'ru',
      date: new Date
    }
  },
  methods:{
    localeRu() {
      this.language = 'ru'
    },
    localeEng() {
      this.language = 'en'
    }
  }
}
</script>

<style>
</style>
