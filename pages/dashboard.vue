<template>
  <div>
    <div class="bg-stone-800 min-h-screen flex flex-col">
      <div class="nav flex justify-center p-5 m-2">
        <p class="text-6xl font-bold text-white border-t-0 border-b-4 border-amber-400 rounded-lg p-5">Dashboard</p>
      </div>
      <div class="blocks flex gap-5 flex-row p-3 m-3 flex-wrap">
        <div class="block cursor-pointer p-12 text-center content-center  m-2 rounded-lg shadow-md bg-stone-700" v-for="block in blocks" :key="block.title">
          <p class="block-title text-2xl font-bold text-white">{{ block.title }}</p>
          <p class="block-description text-lg text-white">{{ block.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>


const blocks = ref([
  {
    title: 'Mathematics',
    description: 'Algebra, Calculus, Statistics',
  },
  {
    title: 'Science',
    description: 'Physics, Chemistry, Biology',
  },
  {
    title: 'Programming',
    description: 'Python, JavaScript, Java',
  },
  {
    title: 'Languages',
    description: 'English, Spanish, French',
  },
  {
    title: 'History',
    description: 'World History, Geography',
  }
])


</script>

<style>

</style>