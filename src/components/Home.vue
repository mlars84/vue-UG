<template>
  <div>
    <h1 v-once>{{ title }}</h1>
    <p>{{ sayHello() }}</p>
    <a :href="link">Google</a>
    <p v-html="finishedLink"></p>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'hello',
      link: 'http://google.com',
      finishedLink: '<a href="http://google.com">Google</a>'
    }
  },
  methods: {
    sayHello () {
      return this.title
    }
  }
}
</script>

<style>
</style>
