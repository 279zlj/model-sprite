<template>
  <div class="hello">
    <model-gltf :backgroundAlpha="bgAlpha"  :rotation="rotation"  @on-load="onLoad" :spritefun="safun" :spritetext="sastatic" :tonealgin="tonealgin"  :ttwoalgin="ttwoalgin" :tcolor="tcolor"  :position="where" :backgroundColor="bgColor" src="../../static/server/server2801.gltf" :cameraPosition="camera" :width="wid" :height="hei"></model-gltf>
  </div>
</template>

<script>
  import ModelGltf from "../assets/3d-text2d/vue-3d/model-gltf";
export default {
  name: 'HelloWorld',
  components: {
    ModelGltf,
  },
  data () {
    return {
      camera: {x: 0, y: 70, z: -280},
      bgAlpha: .3,
      bgColor: '#2E2245',
      wid: 950,
      hei: 443,
      tcontent: '',
      ttitle: '',
      dosome: '',
      sastatic:"CPU温度：30°C，风扇转速：300转",
      safun: "显卡温度：25°C，阵列卡温度：28°C",
      // sacard: this.$store.state.cardtem,
      tonealgin:'bottomLeft',
      ttwoalgin:'bottomRight',
      tcolor:'#FFFFFF',
      rotation: {
        x: 0,
        y: 0,
        z: 0
      },
      where: {x: 0, y: 0, z: -20},
    }
  }
}
</script>

<style scoped>

</style>
