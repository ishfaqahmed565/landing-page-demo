<script setup>
let props = defineProps({
  data: String,
});
console.log(props.data, "value");
let style = `flex ${props.data}  space-y-10 md:space-y-0 md:space-x-20 justify-between  mt-10 padding-x items-center`;
</script>
<template>
  <div :class="style">
    <div class="left lg:w-1/2 flex flex-col flex-1 space-y-3">
      <slot name="left"></slot>
    </div>
    <div class="right lg:w-1/2 flex-col flex-1 space-y-3">
      <slot name="right"></slot>
    </div>
  </div>
</template>
<style scoped></style>
