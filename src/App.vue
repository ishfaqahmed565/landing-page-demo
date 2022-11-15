<script setup>
import {
  NavbarSec,
  HeroSec,
  StatsSec,
  BusinessCard,
  InvoiceCard,
  SwapCard,
  TestimonialSec,
  ClientsSec,
  CTASec,
  FooterSec,
} from "@/components/compImports.js";
</script>

<template>
  <div class="w-full text-white">
    <NavbarSec />
    <div class="main xl:max-w-7xl flex flex-col mx-auto space-y-36">
      <HeroSec />
      <StatsSec />
      <BusinessCard />
      <InvoiceCard />
      <SwapCard />
      <TestimonialSec />
      <ClientsSec />
      <CTASec />
    </div>
    <FooterSec />
  </div>
</template>

<style scoped></style>
