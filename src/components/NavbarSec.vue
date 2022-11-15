<script setup>
let showClose = ref(false);
import { onMounted, ref } from "vue";
let scrolled = ref(0);
let sticky = ref(false);
onMounted(() => {
  function scrolledAmn() {
    scrolled.value = window.pageYOffset;
    if (scrolled.value > 0) {
      sticky.value = true;
    } else if (scrolled.value == 0) {
      sticky.value = false;
    }
    console.log(sticky.value);
  }
  window.addEventListener("scroll", scrolledAmn);
});
</script>
<template>
  <div
    class="px-[2rem] flex items-center justify-between"
    :class="{ sticky: sticky }"
  >
    <img
      src="@/assets/svgs/logo.svg"
      alt="logo"
      class="w-[10rem] h-[5rem] object-contain"
    />
    <nav class="hidden sm:block">
      <ul class="flex space-x-3 text-[15px]">
        <li>
          <a href="#" class="font-normal hover:text-blue-400">Home</a>
        </li>
        <li>
          <a href="#" class="font-normal hover:text-blue-400">About</a>
        </li>
        <li>
          <a href="#" class="font-normal hover:text-blue-400">Features</a>
        </li>
        <li>
          <a href="#" class="font-normal hover:text-blue-400">Solution</a>
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
.sticky {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  background: #0b0a0c;
  z-index: 100;
  border-bottom: 0.1px solid rgb(134, 109, 109);
}
</style>
