<script setup></script>
<template>
  <div
    class="animate-pulse hover:pointer rounded-full relative bottom-2 w-16 h-16 text-center pt-5 text-blue-300 text-[8px] leading-[10px] hidden sm:block border-2 gradient-border"
  >
    <a href="" class="flex flex-col item-center">
      <div class="flex flex items-center mx-auto space-x-1">
        <p>
          <span class="flex items-center">Get</span>
        </p>
        <img
          src="@/assets/svgs/arrow-up.svg"
          alt=""
          class="w-3 h3 object-contain"
        />
      </div>

      <span>Started</span>
    </a>
  </div>
</template>
<style scoped>
.gradient-border {
  border-image: linear-gradient(
    157.81deg,
    #def9fa -43.27%,
    #bef3f5 -21.24%,
    #9dedf0 12.19%,
    #7de7eb 29.82%,
    #5ce1e6 51.94%,
    #33bbcf 90.29%
  );
  border: 1px solid;
  border-radius: 50px;
}
</style>
