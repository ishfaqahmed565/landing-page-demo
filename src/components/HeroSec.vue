<script setup>
import GetStarted from "@/components/GetStarted.vue";
</script>
<template>
  <div
    class="flex sm:flex-row flex-col space-x-2 border padding-x sm:items-center justify-between"
  >
    <div class="right flex-1 flex flex-col space-y-3 pt-[5rem]">
      <div
        class="discount-button px-1 p-1 rounded text-[10px] space-x-1 flex-center bg-[#1c1b22] w-max"
      >
        <img src="@/assets/svgs/discount.svg" alt="dicount" class="w-4 h-4" />
        <p class="text-gray-300 font-[300]">
          <span class="font-semi text-white">20%</span> DICOUNT FOR
          <span class="font-semi text-white">1 MONTH</span>
          ACCOUNT
        </p>
      </div>
      <h2
        class="font-[500] text-[52px] md:text-[72px] leading-[3rem] md:leading-[4rem]"
      >
        <div class="flex items-center relative">
          <div>
            The Next <br />
            <span class="font-semibold text-gradient">Generation</span>
          </div>

          <GetStarted />
        </div>

        Payment Method
      </h2>
      <div>
        <p
          class="font-thin text-dimWhite text-[15px] leading-[16.8px] max-w-[470px] mt-5 font-[200]"
        >
          Our team of experts uses a methodology to identify the credit cards
          most likely to fit your needs. We examine annual percentage rates,
          annual fees.
        </p>
      </div>
    </div>
    <!--Right side ends here-->
    <div class="left md:my-0 my-10 relative">
      <img
        src="@/assets/images/robot.png"
        class="w-[100%] h[100%] lg:max-w-lg"
      />
    </div>
    <!--Left side ends here-->
  </div>
</template>
<style scoped>
.gradient-border {
  border-image: linear-gradient(to right, #2980b9, #6dd5fa, #ffffff) border-box;
  border: 1px solid;
  border-radius: 50px;
}
</style>
