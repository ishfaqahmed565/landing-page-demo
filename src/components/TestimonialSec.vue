<script setup>
import InfoCard from "@/components/InfoCard.vue";
</script>
<template>
  <div class="flex flex-col space-y-10 mt-10">
    <InfoCard data="md:flex-row flex-col ">
      <template v-slot:left>
        <h3 class="header2-style">
          What people are saying <br />about us
        </h3></template
      >
      <template v-slot:right>
        <p class="paragraph-style mr-10 flex-none">
          Everything you need to accept card payments and grow your business
          anywhere on the planet.
        </p>
      </template>
    </InfoCard>
    <div
      class="flex md:flex-row flex-col md:space-x-3 space-y-3 md:space-y-0 padding-x"
    >
      <div
        class="rounded-xl black-gradient flex flex-col px-5 py-10 justify-between md:w-1/3 w-full items-center md:items-start"
      >
        <img
          src="@/assets/svgs/quotes.svg"
          alt=""
          class="w-[20px] self-start"
        />
        <p class="paragraph-style">
          Money is only a tool. It will take you wherever you wish, but it will
          not replace you as the driver.
        </p>
        <div class="flex space-x-3 items-center">
          <img
            src="@/assets/images/people01.png"
            alt=""
            class="w-8 h-8 object-contain"
          />
          <div>
            <h4 class="font-light">Herman Joseph</h4>
            <p class="font-thin text-[9px] text-gray-200">Founder & Leader</p>
          </div>
        </div>
      </div>
      <div
        class="rounded-xl black-gradient flex flex-col px-5 py-10 justify-between md:w-1/3 w-full items-center md:items-start"
      >
        <img
          src="@/assets/svgs/quotes.svg"
          alt=""
          class="w-[20px] self-start"
        />
        <p class="paragraph-style">
          Money makes your life easier. If you're lucky to have it, you're
          lucky.
        </p>
        <div class="flex space-x-3 items-center">
          <img
            src="@/assets/images/people02.png"
            alt=""
            class="w-8 h-8 object-contain"
          />
          <div>
            <h4 class="font-light">Steve Mark</h4>
            <p class="font-thin text-[9px] text-gray-200">Founder & Leader</p>
          </div>
        </div>
      </div>
      <div
        class="rounded-xl black-gradient flex flex-col px-5 py-10 justify-between md:w-1/3 w-full items-center md:items-start"
      >
        <img
          src="@/assets/svgs/quotes.svg"
          alt=""
          class="w-[20px] self-start"
        />
        <p class="paragraph-style">
          It is usually people in the money business, finance, and international
          trade that are really rich.
        </p>
        <div class="flex space-x-3 items-center">
          <img
            src="@/assets/images/people03.png"
            alt=""
            class="w-8 h-8 object-contain"
          />
          <div>
            <h4 class="font-light">Steve Mark</h4>
            <p class="font-thin text-[9px] text-gray-200">Founder & Leader</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped></style>
