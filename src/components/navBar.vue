<script>
export default {
  data() {
    return {
      nav: false,
      links: [
        {
          id: 1,
          link: "home",
        },
        {
          id: 2,
          link: "about",
        },
        {
          id: 3,
          link: "portfolio",
        },
        {
          id: 4,
          link: "experience",
        },
        {
          id: 5,
          link: "contact",
        },
      ],
    };
  },
  methods: {
    setNav() {
      this.nav = !this.nav;
      console.log(this.nav);
    },
  },
};
</script>

<template>
  <div
    class="flex justify-between items-center w-full h-20 bg-black px-4 text-white fied"
  >
    <div class="text-5xl font-signature ml-2">Nico</div>
    <div class="w-full">
      <ul class="hidden md:flex justify-end">
        <li
          class="px-4 cursor-pointer capitalize font-medium text-gray-500 hover:scale-105 duration-200"
          v-for="(item, index) in links"
          :key="index"
        >
          {{ item.link }}
        </li>
      </ul>
    </div>
    <div>
      <i
        class="fa-solid fa-bars text-2xl relative cursor-pointer pr-4 z-10 text-gray-500 md:hidden"
        @click="setNav()"
        :class="nav ? 'hidden' : ''"
      ></i>
      <i
        class="fa-solid fa-xmark text-2xl relative cursor-pointer pr-4 z-10 text-gray-500 md:hidden"
        @click="setNav()"
        :class="nav ? '' : 'hidden'"
      ></i>
    </div>

    <ul
      v-if="nav"
      class="flex flex-col justify-center items-center absolute top-0 left-0 w-full h-full bg-gradient-to-b from-black to-gray-800 text-gray-500"
    >
      <li
        class="px-4 cursor-pointer capitalize py-6 text-4xl hover:scale-105 duration-200"
        v-for="(item, index) in links"
        :key="index"
      >
        {{ item.link }}
      </li>
    </ul>
  </div>
</template>

<style></style>
