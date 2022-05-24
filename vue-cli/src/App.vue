<template>
  <div>
    <AppHeader v-bind:propsdata="str" v-on:renew="renewStr" />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {
  data() {
    return {
      str: 'Header1'
    }
  },
  components: {
    AppHeader
  },
  methods: {
    renewStr() {
      this.str = 'wow';
    }
  }
}
</script>

<style>

</style>