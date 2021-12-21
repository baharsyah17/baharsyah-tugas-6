<template>
  <div>
    <div
      class="bg-blue-200 fixed grid grid-cols-1 rounded-md lg:grid-cols-4 gap-7 justify-content-center mt-20 mr-20 ml-20 p-8"
    >
      <div
        class="relative bg-purple-600 text-white p-8 rounded-lg lg:col-span-2"
      >
        <img
          :src="kutip"
          alt="tanda Kutip"
          class="absolute top-2 right-4 z-0"
        />
        <div class="relative z-10 flex justify start space-x-3">
          <img
            :src="studentData[0].image"
            alt="Daniel"
            class="h-8 w-8 rounded-full border-2 border-purple-400"
          />
          <div>
            <h2 class="font-bold text-sm">{{ studentData[0].name }}</h2>
            <h3 class="text-xs">{{ status }}</h3>
          </div>
        </div>
        <p class="relative z-10 mt-4 font-bold text-xl">
          {{ studentData[0].quote }}
        </p>
        <p class="mt-4 text-sm">{{ studentData[0].opinion }}</p>
      </div>
      <div class="relative bg-gray-600 text-white p-8 rounded-lg">
        <div class="relative z-10 flex justify start space-x-3">
          <img
            :src="studentData[1].image"
            alt="jonathan"
            class="h-8 w-8 rounded-full border-2 border-purple-400"
          />
          <div>
            <h2 class="font-bold text-sm">{{ studentData[1].name }}</h2>
            <h3 class="text-xs">{{ status }}</h3>
          </div>
        </div>
        <p class="relative z-10 mt-4 font-bold text-xl">
          {{ studentData[1].quote }}
        </p>
        <p class="mt-4 text-sm">{{ studentData[1].opinion }}</p>
      </div>
      <div class="relative bg-white text-black p-8 rounded-lg lg:row-start-2">
        <div class="relative z-10 flex justify start space-x-3">
          <img
            :src="studentData[2].image"
            alt="jeanette"
            class="h-8 w-8 rounded-full border-2 border-purple-400"
          />
          <div>
            <h2 class="font-bold text-sm">{{ studentData[2].name }}</h2>
            <h3 class="text-xs">{{ status }}</h3>
          </div>
        </div>
        <p class="relative z-10 mt-4 font-bold text-xl">
          {{ studentData[2].quote }}
        </p>
        <p class="mt-4 text-sm">{{ studentData[2].opinion }}</p>
      </div>
      <div class="relative bg-black text-white p-8 rounded-lg lg:col-span-2">
        <div class="relative z-10 flex justify start space-x-3">
          <img
            :src="studentData[3].image"
            alt="jeanette"
            class="h-8 w-8 rounded-full border-2 border-purple-400"
          />
          <div>
            <h2 class="font-bold text-sm">{{ studentData[3].name }}</h2>
            <h3 class="text-xs">{{ status }}</h3>
          </div>
        </div>
        <p class="relative z-10 mt-4 font-bold text-xl">
          {{ studentData[3].quote }}
        </p>
        <p class="mt-4 text-sm">{{ studentData[3].opinion }}</p>
      </div>
      <div
        class="relative bg-white text-black p-8 rounded-lg lg:row-span-2 lg:row-start-1 lg:col-start-4"
      >
        <div class="relative z-10 flex justify start space-x-3">
          <img
            :src="studentData[4].image"
            alt="jeanette"
            class="h-8 w-8 rounded-full border-2 border-purple-400"
          />
          <div>
            <h2 class="font-bold text-sm">{{ studentData[4].name }}</h2>
            <h3 class="text-xs">{{ status }}</h3>
          </div>
        </div>
        <p class="relative z-10 mt-4 font-bold text-xl">
          {{ studentData[4].quote }}
        </p>
        <p class="mt-4 text-sm">{{ studentData[4].opinion }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    status: {
      type: String,
      default: "",
    },
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
