<script setup></script>
<template>
  <footer
    class="flex flex-col = px-[2rem] py-[5rem] bg-[#0B0A0C] w-full space-y-10 mt-36"
  >
    <div class="flex md:flex-row flex-col space-y-10 md:space-y-0">
      <div
        class="flex flex-col items-center md:items-start justify-between md:w-3/6 space-y-10"
      >
        <img
          src="@/assets/svgs/logo.svg"
          alt=""
          class="w-[10rem] object-contain"
        />
        <p class="paragraph-style">
          A new way to make the payments easy, reliable and secure.
        </p>
      </div>

      <div
        class="links flex md:space-x-20 flex-col md:flex-row space-y-5 md:space-y-0"
      >
        <div
          class="flex flex-col items-center md:items-start space-y-6 text-white"
        >
          <strong
            >Useful Links
            <hr
          /></strong>
          <ul
            class="flex flex-row md:flex-col w-full justify-between flex-wrap"
          >
            <li class="paragraph-style">Content</li>
            <li class="paragraph-style">How it Works</li>
            <li class="paragraph-style">Create</li>
            <li class="paragraph-style">Explore</li>
            <li class="paragraph-style">Terms & Service</li>
          </ul>
        </div>

        <div
          class="flex flex-col items-center md:items-start space-y-6 text-white"
        >
          <strong
            >Community
            <hr
          /></strong>
          <ul
            class="flex flex-row md:flex-col w-full justify-between flex-wrap"
          >
            <li class="paragraph-style">Help Center</li>
            <li class="paragraph-style">Partners</li>
            <li class="paragraph-style">Suggestions</li>
            <li class="paragraph-style">Blog</li>
            <li class="paragraph-style">Newsletter & More</li>
          </ul>
        </div>

        <div
          class="flex flex-col items-center md:items-start space-y-6 text-white"
        >
          <strong
            >Partner
            <hr
          /></strong>
          <div>
            <ul class="flex flex-row md:flex-col w-full flex-wrap">
              <li class="paragraph-style">Our Partner</li>
              <li class="paragraph-style ml-10 md:ml-0">Become a Partner</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <hr />
    <div class="flex justify-between items-center flex-col sm:flex-row">
      <p class="text-[11px] font-thin">
        Copyright © 2021 HooBank. All Rights Reserved.
      </p>
      <div class="flex space-x-5">
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-facebook"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-linkedin"></i>
      </div>
    </div>
  </footer>
</template>
<style scoped></style>
