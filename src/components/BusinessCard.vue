<script setup>
import ButtonItem from "@/components/ButtonItem.vue";
import InfoCard from "@/components/InfoCard.vue";
import DescriptionCard from "@/components/DescriptionCard.vue";
</script>
<template>
  <InfoCard data="md:flex-row flex-col">
    <template v-slot:left>
      <DescriptionCard>
        <template v-slot:header>
          You do the business <br class="hidden sm:block" />
          we'll handle the money
        </template>
        <template v-slot:paragraph>
          With the right credit card, you can improve your financial life by
          building credit, earning rewards and saving money. But with hundreds
          of credit cards on the market.
        </template>
      </DescriptionCard>

      <ButtonItem />
    </template>
    <template v-slot:right>
      <div
        class="flex items-center space-x-2 rounded-2xl py-2 px-5 black-gradient"
      >
        <div class="bg-[#09977C] bg-opacity-20 rounded-full py-2 px-2">
          <img src="@/assets/svgs/Star.svg" alt="" class="w-[35px] h-[35px]" />
        </div>

        <div class="flex flex-col">
          <h4 class="font-semibold">Rewards</h4>
          <p class="paragraph-style">
            The best credit cards offer some tantalizing combinations of
            promotions and prizes
          </p>
        </div>
      </div>
      <div
        class="flex items-center space-x-2 rounded-2xl py-2 px-5 black-gradient"
      >
        <div class="bg-[#09977C] bg-opacity-20 rounded-full py-2 px-2">
          <img
            src="@/assets/svgs/Shield.svg"
            alt=""
            class="w-[35px] h-[35px]"
          />
        </div>
        <div class="flex flex-col">
          <h4 class="font-semibold">100% Secured</h4>
          <p class="paragraph-style">
            We take proactive steps make sure your information and transactions
            are secure.
          </p>
        </div>
      </div>
      <div
        class="flex items-center space-x-2 rounded-2xl py-2 px-5 black-gradient"
      >
        <div class="bg-[#09977C] bg-opacity-20 rounded-full py-2 px-2">
          <img src="@/assets/svgs/Send.svg" alt="" class="w-[35px] h-[35px]" />
        </div>

        <div class="flex flex-col">
          <h4 class="font-semibold">Balance Transfer</h4>
          <p class="paragraph-style">
            A balance transfer credit card can save you a lot of money in
            interest charges.
          </p>
        </div>
      </div>
    </template>
  </InfoCard>
</template>
<style scoped></style>
