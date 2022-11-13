<script setup>
import DescriptionCard from "@/components/DescriptionCard.vue";
import InfoCard from "@/components/InfoCard.vue";
import ButtonItem from "@/components/ButtonItem.vue";
</script>

<template>
  <InfoCard data="md:flex-row flex-col">
    <template v-slot:left>
      <DescriptionCard>
        <template v-slot:header
          >Find a better card deal<br class="hidden sm:block" />
          in few easy steps.
        </template>
        <template v-slot:paragraph
          >Arcu tortor, purus in mattis at sed integer faucibus. Aliquet quis
          aliquet eget mauris tortor.ç Aliquet ultrices ac, ametau.
        </template>
      </DescriptionCard>
      <ButtonItem />
    </template>
    <template v-slot:right>
      <img
        src="@/assets/images/card.png"
        alt=""
        class="w-full object-fill mt-10 sm:mt-0"
      />
    </template>
  </InfoCard>
</template>
<style scoped></style>
