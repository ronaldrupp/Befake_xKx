<script>
export default {
  props: ["realmoji"],
};
</script>
<template>
  <div class="flex items-center mb-2">
    <div class="relative">
      <img
        referrerpolicy="no-referrer"
        v-bind:src="realmoji.uri"
        class="w-24 rounded-[50%]" />

      <span class="absolute top-[50px] left-[60px] text-5xl"
        >{{ realmoji.emoji }}
      </span>
    </div>
    <span class="font-bold ml-4">{{ realmoji.userName }}</span>
  </div>
</template>
