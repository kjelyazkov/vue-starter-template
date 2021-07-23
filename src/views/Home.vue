<template>
  <div class="h-screen w-full flex flex-col overflow-hidden">
    <div class="p-3 flex justify-between items-center">
      <h1 class="text-2xl font-bold first-letter:text-red-600">RIDOTAX</h1>
      <div class="flex gap-2 text-2xl">
        <div class="px-2 py-1 rounded-md">
          <i class="fas fa-cog"></i>
        </div>
        <div class="px-2 py-1 rounded-md">
          <i class="fas fa-bell"></i>
        </div>
      </div>
    </div>
    <div class="w-full flex flex-nowrap overflow-x-scroll no-scroll p-4 gap-4">
      <div
        class="
          w-[100px]
          h-[125px]
          grid
          place-content-center
          text-3xl
          bg-gray-500
          text-gray-400
          rounded-md
          flex-shrink-0
        "
      >
        <i class="fas fa-plus"></i>
      </div>
      <div
        class="
          w-[100px]
          h-[125px]
          flex
          text-3xl
          bg-gray-600
          rounded-md
          text-[1.2rem]
          leading-none
          p-2
          truncate
          flex-shrink-0
        "
        v-for="(car, index) in 7"
        :key="index"
      >
        Volkswaggen
      </div>
    </div>
    <div class="flex flex-col gap-2 flex-1 overflow-y-scroll no-scroll">
      <div
        v-for="(fee, index) in 12"
        :key="index"
        class="w-full bg-gray-300 p-4 flex flex-col gap-4"
      >
        <div class="text-xl">Item {{ index + 1 }}</div>
        <div class="flex justify-between items-center">
          <div>Insurance</div>
          <div>2 days left</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
