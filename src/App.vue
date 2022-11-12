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
  <div class="xl:max-w-7xl w-full text-white border mx-auto">
    <div class="w-full">
      <div><NavbarSec /></div>
      <div><HeroSec /></div>
      <div><StatsSec /></div>
      <div><BusinessCard /></div>
      <div><InvoiceCard /></div>
      <div><SwapCard /></div>
      <div><TestimonialSec /></div>
      <div><ClientsSec /></div>
      <div><CTASec /></div>
      <div><FooterSec /></div>
    </div>
  </div>
</template>

<style scoped></style>
