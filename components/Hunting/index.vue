<script setup>
import Lottie from "lottie-web";
import animationData from "@/public/assets/hunting.json"

const lottieContainer = ref(null);

onMounted(() => {
  Lottie.loadAnimation({
    container: lottieContainer.value,
    renderer: "svg",
    loop: true,
    autoplay: true,
    animationData: animationData,
  })
})

</script>


<template>
  <div class="h-full w-full flex flex-col items-center justify-center">
    <div ref="lottieContainer"/>
  </div>
</template>