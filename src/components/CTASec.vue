<script setup>
import ButtonItem from "@/components/ButtonItem.vue";
</script>
<template>
  <div
    class="flex px-5 py-8 rounded-xl black-gradient md:flex-row flex-col justify-between mt-[7rem] mx-[2rem] lg:mx-[0rem] items-center"
  >
    <div class="flex flex-col space-y-4">
      <h4 class="header2-style">Let’s try our service now!</h4>
      <p class="paragraph-style">
        Everything you need to accept card payments and grow your business
        anywhere on the planet.
      </p>
    </div>
    <div class="md:mr-24 mt-10 md:mt-0">
      <ButtonItem />
    </div>
  </div>
</template>
<style scoped>
.black-gradient {
  background: linear-gradient(
    144.39deg,
    #ffffff -278.56%,
    #6d6d6d -78.47%,
    #11101d 91.61%
  );
  backdrop-filter: blur(5px);
}
</style>
