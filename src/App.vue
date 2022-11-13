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
  <div class="xl:max-w-7xl w-full text-white mx-auto">
    <NavbarSec />
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
</template>

<style scoped></style>
