<template>
  <div id="app">
    <div id="nav">
      <b-navbar type="dark" variant="dark">
    <b-navbar-brand class="p-4" ><b><b>SushiZone</b></b></b-navbar-brand>
  </b-navbar>
  <vue-qrcode class="qr"  value="https://youthful-dijkstra-9086b2.netlify.app/"/>
  <p class="text">Scan QR Code</p>
    </div>
    <router-view/>
  </div>
</template>

<script>
import VueQrcode from 'vue-qrcode'

export default {
  components: {
    VueQrcode,
  },
  
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.text{
  text-align: center;
  line-height: 860px;
  position: inherit;
    top:  70%;
    left: 50%;
    transform: translate(-50%,-50%);
}

.qr{
  position: absolute;
    top:  50%;
    left: 50%;
    transform: translate(-50%,-50%);
    block-size: 16rem;
}
</style>
