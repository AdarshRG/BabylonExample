<template>
 <div>
  <h3>Babylon Examples</h3>
  <canvas></canvas>
 </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { BasicScene } from "@/BabylonExamples/BasicScene";


export default defineComponent({
  name: 'BabylonExamples',
 mounted(){
const canvas=document.querySelector("canvas")!
new BasicScene(canvas)
 }
});
</script>


<style scoped>
canvas{
  width:100%;
  height:80%;
}
</style>
