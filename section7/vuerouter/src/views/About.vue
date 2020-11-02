<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button @click="checkRouteInfo">ルート情報</button>
  </div>
</template>


<script>
export default {
  name: 'About',
  methods: {
    checkRouteInfo() {
      console.log(this.$route)
      console.log(this.$router)
    }
  }
}
</script>
