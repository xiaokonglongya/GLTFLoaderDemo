<template>
  <div style="width: 1200px; height: 700px">
    <model-viewer
      id="model-viewer"
      :src="MODEL"
      ar
      ar-modes="scene-viewer quick-look"
      camera-controls
      touch-action="pan-y"
      alt="A 3D model of an astronaut"
      shadow-intensity="2"
      auto-rotate
      disable-pan
      skybox-height="2m"
      max-camera-orbit="auto 90deg auto"
    >
    </model-viewer>
  </div>
</template>
<script setup>
import MODEL from '../assets/ali.glb'
</script>
<style>
model-viewer {
  position: relative;
  background: transparent;
  width: 100%;
  height: 100%;
}
</style>
