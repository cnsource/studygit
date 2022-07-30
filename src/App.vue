<script setup>
import { ref } from 'vue';

const isOpen = ref(false)

function changeModetoDark(){
  let root = document.getElementById("root");
  root.classList.add('dark')
}

function changeModetoLight(){
  let root = document.getElementById("root");
  root.classList.remove('dark')
}

function showName(){
  alert('你好小刘同学')
}
</script>

<template>
    <div class="w-full h-screen bg-sky-400 dark:bg-slate-300 flex justify-center items-center">
        <button @click="showName" class="px-4 py-1.5 border-white border-2 text-white">点击输出你好小刘同学</button>
        <button @click="changeModetoDark" class="px-4 py-1.5 border-white border-2 text-white">切换暗模式</button>
        <button @click="changeModetoLight" class="px-4 py-1.5 border-white border-2 text-white">切换亮模式</button>
    </div>
</template>

<style scoped>

</style>
