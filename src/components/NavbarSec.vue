<script setup>
import { ref } from "vue";
let showClose = ref(false);
</script>
<template>
  <div class="padding-x flex items-center justify-between">
    <img
      src="@/assets/svgs/logo.svg"
      alt="logo"
      class="w-[10rem] h-[5rem] object-contain"
    />
    <nav class="hidden sm:block">
      <ul class="flex space-x-3 text-[12px]">
        <li>
          <a href="#" class="font-thin hover:text-blue-400">Home</a>
        </li>
        <li>
          <a href="#" class="font-thin hover:text-blue-400">About</a>
        </li>
        <li>
          <a href="#" class="font-thin hover:text-blue-400">Features</a>
        </li>
        <li>
          <a href="#" class="font-thin hover:text-blue-400">Solution</a>
        </li>
      </ul>
    </nav>
    <div class="relative sm:hidden">
      <button class="sm:hidden">
        <img
          src="@/assets/svgs/menu.svg"
          alt="menu logo"
          @click="showClose = true"
          v-show="!showClose"
        />
        <img
          src="@/assets/svgs/close.svg"
          alt="menu logo"
          @click="showClose = false"
          v-show="showClose"
        />
      </button>
      <Transition name="wrapper">
        <div
          class="min-w-[120px] absolute black-gradient rounded-lg right-0 top-10 z-50"
          v-show="showClose"
        >
          <ul class="flex flex-col space-y-2 text-[12px] py-3 px-3">
            <li>
              <a href="#" class="font-thin hover:text-blue-400">Home</a>
            </li>
            <li>
              <a href="#" class="font-thin hover:text-blue-400">About</a>
            </li>
            <li>
              <a href="#" class="font-thin hover:text-blue-400">Features</a>
            </li>
            <li>
              <a href="#" class="font-thin hover:text-blue-400">Solution</a>
            </li>
          </ul>
        </div>
      </Transition>
    </div>
  </div>
</template>
<style scoped>
.black-gradient {
  background: linear-gradient(
    144.39deg,
    #ffffff -278.56%,
    #6d6d6d -78.47%,
    #11101d 91.61%
  );
  backdrop-filter: blur(5px);
}
.wrapper-enter-active {
  animation-name: finished;
  animation-duration: 0.5s;
}
.wrapper-leave-active {
  animation: finished 0.2s reverse;
}
@keyframes finished {
  0% {
    opacity: 0;
    top: 5rem;
  }

  100% {
    opacity: 1;
    top: 2.5rem;
  }
}
</style>
