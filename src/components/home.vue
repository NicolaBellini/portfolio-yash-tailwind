<script>
export default {};
</script>

<template>
  <div
    class="scroll-smooth h-screen w-full bg-gradient-to-b from-black via-black to-gray-800"
  >
    <div
      class="max-w-screen-xl mx-auto flex flex-col items-center justify-around px-4 text-white h-full md:flex-row"
    >
      <div class="flex flex-col justify-center h-full">
        <h2 class="text-4xl md:text-7xl font-bold max-w-md">
          Sono un Full-Stack Developer
        </h2>
        <p class="text-gray-500 max-w-md">
          Web developer sempre alla ricerca di nuovi modi per sfruttare la
          creatività e le competenze tecniche per fare la differenza. Motivato
          dalla possibilità di contribuire al benessere della comunità, sono
          entusiasta di collaborare su progetti che abbiano un impatto positivo
          e significativo.
        </p>

        <div>
          <button
            class="group bg-gradient-to-r from-cyan-500 to-blue-500 py-3 px-6 rounded-xl w-fit"
          >
            Portfolio
            <span>
              <i
                class="fa-solid fa-arrow-right group-hover:rotate-90 duration-150 text-lg ml-1"
              ></i>
            </span>
          </button>
        </div>
      </div>
      <div>
        <img
          src="/public/img/IMG_2838.jpeg"
          class="rounded-3xl mx-auto max-h-[600px] w-2/3 md:w-full"
          alt="NicolaBellini"
        />
      </div>
    </div>
  </div>
</template>

<style></style>
