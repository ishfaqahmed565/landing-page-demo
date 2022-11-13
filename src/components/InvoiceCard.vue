<script setup>
import InfoCard from "@/components/InfoCard.vue";
import DescriptionCard from "@/components/DescriptionCard.vue";
</script>
<template>
  <InfoCard data="md:flex-row flex-col-reverse">
    <template v-slot:left>
      <img
        src="@/assets/images/bill.png"
        alt=""
        class="w-full object-contain mt-10 sm:mt-0"
      />
    </template>
    <template v-slot:right>
      <DescriptionCard>
        <template v-slot:header
          >Easily control your <br class="hidden sm:block" />
          billing & invoicing.
        </template>
        <template v-slot:paragraph
          >Elit enim sed massa etiam. Mauris eu adipiscing ultrices ametodio
          aenean neque. Fusce ipsum orci rhoncus aliporttitor integer platea
          placerat.
        </template>
      </DescriptionCard>
      <div class="flex space-x-3">
        <img src="@/assets/svgs/apple.svg" alt="" />
        <img src="@/assets/svgs/google.svg" alt="" />
      </div>
    </template>
  </InfoCard>
</template>
<style scoped></style>
