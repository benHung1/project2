<script setup>
import { ref } from "vue";

const props = defineProps({
  isOpen: {
    type: Boolean,
    default: false,
  },
});

const emit = defineEmits(["close"]);

const isClose = () => {
  emit("close");
};

const data = ref([
  { title: "獎項", content: "活動編號" },
  { title: "康生十足美人美腿機(1名)", content: "222729" },
  {
    title: "7-11購物金50元(10名)",
    content:
      "218265、214476、2172 \r\n 219972、222174、210099 \r\n 218841、221379、221715、21997",
  },
  {
    title: "必勝客六吋個人鬆厚比薩即享卷(3名)",
    content: "221493、211542、213687 ",
  },
  { title: "威秀影城電影票兌換卷乙張(2名)", content: "210453、218466" },
]);
</script>

<template lang="">
  <div
    class="w-full h-screen bg-black opacity-80 z-10 fixed top-0"
    v-if="isOpen"
    @click="isClose"
  />
  <div
    v-if="isOpen"
    class="border-blue-600 border-2 absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 bg-white h-[60vh] overflow-y-auto py-4 px-12 rounded-xl max-w-[1440px] w-[80%] flex flex-col items-center text-center z-40"
  >
    <button type="" class="block ml-auto bg-red-500" @click="isClose">
      close
    </button>
    <h1>
      感謝您的熱情參與，【月來月好玩、有點送虎禮】五月份月月抽獎項已抽出。<br />
      1.主辦單位會發送中獎通知信件至「電子信箱」，請依照通知中說明於期限內完成兌獎步驟。<br />
      2.若因資料填寫有誤致無法聯繫與領取獎項，視同放棄中獎資格不得異議。<br />
    </h1>
    <h1 class="mt-[20px] text-lg">月月抽得獎名單</h1>
    <hr class="border-[1px] border-gray-400 w-full mb-[10px]" />
    <hr class="border-[1px] border-gray-400 w-full" />
    <h1 class="my-[20px] text-2xl">
      5月份得獎名單<span class="text-red-600"
        >兌獎期間 111年06月10日-06月24日</span
      >
    </h1>
    <hr class="border-[1px] border-gray-400 w-full" />
    <h1 class="text-white bg-black rounded-xl p-4 my-[20px]">
      活動期間111年05月09日-05月31日
    </h1>
    <hr class="border-[1px] border-gray-400 w-full" />
    <div v-for="(item, index) in data" :key="index" class="mt-[20px]">
      <h1 class="bg-blue-300 rounded-lg p-4">{{ item.title }}</h1>
      <pre>{{ item.content }}</pre>
    </div>
  </div>
</template>
<style>
::-webkit-scrollbar {
  display: none;
}
</style>
