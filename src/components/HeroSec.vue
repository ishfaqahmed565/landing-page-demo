<script setup></script>
<template>
  <div class="flex border padding-x">
    <div class="right flex flex-col space-y-3 pt-[5rem]">
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
      <h2 class="font-[500] text-4xl leading-[3rem]">
        <div class="flex items-center space-x-12 relative">
          <div>
            The Next <br />
            <span class="font-semibold text-4xl text-gradient">Generation</span>
          </div>

          <div
            class="hover:animate-pulse hover:pointer rounded-full relative bottom-2 w-16 h-16 text-center pt-5 text-blue-300 text-[8px] leading-[10px] hidden sm:block border-2 gradient-border"
          >
            <a href="">
              <span class="flex items-center"
                >Get
                <img
                  src="@/assets/svgs/arrow-up.svg"
                  alt=""
                  class="w-5 h5"
                /> </span
              ><br />
              <span>Started</span>
            </a>
          </div>
        </div>

        Payment Method
      </h2>
      <div>
        <p class="text-[11px] w-[17.9rem] mt-5 font-[200]">
          Our team of experts uses a methodology to identify the credit cards
          most likely to fit your needs. We examine annual percentage rates,
          annual fees.
        </p>
      </div>
    </div>
  </div>
</template>
<style scoped>
.gradient-border {
  border-image: linear-gradient(to right, #2980b9, #6dd5fa, #ffffff) border-box;
  border: 1px solid;
  border-radius: 50px;
}
</style>
