<template>
  <div>
    <div class="relative z-10 flex justify start space-x-3">
      <img
        :src="studentData.image"
        :alt="studentData.name"
        class="h-14 w-14 rounded-full border-2 border-purple-400"
      />
      <div>
        <h2 class="font-bold text-lg">{{ studentData.name }}</h2>
        <h3 class="text-base">{{ studentData.status }}</h3>
      </div>
    </div>
    <p class="relative z-10 mt-4 font-bold text-2xl">
      {{ studentData.quotes }}
    </p>
    <p class="mt-4 text-xl">{{ studentData.opinion }}</p>
  </div>
</template>

<script>
export default {
  props: {
    kutip: {
      type: String,
      default: "",
    },
    studentData: {
      type: Array,
      default: [],
    },
  },
};
</script>

<style></style>
