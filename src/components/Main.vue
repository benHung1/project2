<script setup>
import Popup from "../components/Popup.vue";
</script>

<template lang="">
  <Popup />
  <div
    class="w-full flex justify-center flex-col items-center bg-[url('https://acts.setn.com/event/setnappcoin/images/bg-blue.png')] bg-no-repeat bg-center bg-cover bg-[#f5f5dc]"
  >
    <div class="mt-[20px] relative">
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
      class="max-w-[396px] max-h-[130px] md:mb-[250px] mb-[310px] w-full"
    />
  </div>
  <div class="flex justify-center flex-col bg-[#0e478c] fixed bottom-0 w-full">
    <div class="md:flex md:justify-center m-auto py-[15px]">
      <img
        alt=""
        src="../assets/btn-1.png"
        class="max-w-[303px] max-h-[96px] md:mr-[20px] mt-[5px]"
      />
      <img
        alt=""
        src="../assets/btn-2.png"
        class="max-w-[303px] max-h-[96px] my-[5px]"
      />
    </div>
    <h1 class="text-center text-white text-base">
      活動日期:2022/6/10至2022/6/30<br />
      參加資格及辦法:下載三立新聞網APP看新聞，於活動期間登錄即可抽精美好禮
    </h1>
  </div>
</template>
<style lang=""></style>
