<script setup>
import { ref } from "vue";
import Popup from "./Popup";

const isOpen = ref(false);

const Opened = () => {
  isOpen.value = true;
};
</script>

<template lang="">
  <Popup :isOpen="isOpen" @close="isOpen = false" />
  <div
    class="w-full flex justify-center flex-col items-center bg-[url('https://acts.setn.com/event/setnappcoin/images/bg-blue.png')] bg-no-repeat bg-center bg-cover bg-[#f5f5dc]"
  >
    <div class="mt-[20px] relative cursor-pointer" @click="Opened">
      <img src="../assets/prize-list-btn.png" alt="error" />
      <img
        src="../assets/finger.png"
        alt=""
        class="absolute top-3 left-[75%]"
      />
    </div>
    <img
      src="../assets/main-title.png"
      alt=""
      class="max-w-[747px] max-h-[307px] mt-[20px] mb-[100px] w-full"
    />
    <a
      target="_blank"
      href="http://isetevent-new-366957244.ap-northeast-1.elb.amazonaws.com/shareApp/"
    >
      <img
        src="../assets/icon.png"
        alt=""
        class="fixed top-2/4 right-0 -translate-y-2/4"
      />
    </a>
  </div>
  <div class="flex flex-col items-center bg-[#f5f5dc]">
    <img
      src="../assets/prize-win.png"
      alt=""
      class="max-w-[510px] max-h-[709px] w-full -mt-16"
    />
    <img
      src="../assets/coin.png"
      alt=""
      class="max-w-[396px] max-h-[130px] w-full"
    />
  </div>
</template>
<style lang=""></style>
