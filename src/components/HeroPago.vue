<template>
  <section
    id="hero"
    class="relative"
  >
    <div
      id="hero-message-bar"
      class="
        flex
        absolute
        top-0
        left-0
        py-4
        w-full
        z-20
        gap-4
        items-center
        justify-center
        text-white
        bg-[#1A1E89]/60
        backdrop-blur
        backdrop-saturate-150
      "
    >
      <img
        src="@/assets/icons/truck.svg"
        alt=""
        class="w-[30px] h-[18px]"
      />
      <p class="text-sm leading-6 lg:text-xl bg-transparent">
        ¡Contrata hoy y obtén <span class="font-bold">los mejores beneficios</span>!
      </p>
    </div>
    <section
      id="hero-carousel"
      class=" rounded-b-[56px]"
    >
      <div
        id="hero-carousel-sliders"
        class="flex w-full"
      >
        <div class="w-1/2 flex">
          <div class="m-auto lg:max-w-[465px] lg:mt-35 lg:mb-20">
            <h2 class="text-white font-light leading-12 lg:text-[40px]">
              Hazte cliente empresa del Banco de Chile
              <span class="font-bold">y obtén tu producto a costo $0*</span>
            </h2>
            <div class="flex gap-6 mt-10">
              <button class="py-4 px-6 bg-btn-fill text-btn-fill-text font-bold text-sm leading-6 text-center uppercase rounded-full cursor-pointer lg:w-[198px]">
                <p>QUIERO CONTRATAR</p>
              </button>
              <button class="py-4 px-6 bg-transparent text-white font-bold text-sm leading-6 text-center uppercase rounded-full border-2 cursor-pointer lg:w-[206px]">
                <p>Nuestras tarifas</p>
              </button>
            </div>
            <div id="hero-carousel-controls-desktop" class="w-full hidden gap-3 mt-15 lg:flex">
              <img class="user-none self-center cursor-pointer rotate-180" src="@/assets/icons/arrow-hero-alt.svg" alt="slider anterior" />
              <img class="self-center cursor-pointer" src="@/assets/icons/arrow-hero-alt.svg" alt="slider siguiente" />
              <img class="self-center cursor-pointer" src="@/assets/icons/pause-hero.svg" alt="pausar slider" />
            </div>
          </div>
        </div>
        <div class="w-1/2 relative flex items-center overflow-hidden">
          <img
            src="@/assets/images/bg-shape.svg"
            alt=""
            class="absolute top-[-40%] right-[-25%] rotate-[-0deg] opacity-80 z-0 pointer-events-none"
          />
          <div class="relative z-10 lg:mt-15">
            <img
              src="@/assets/images/person-fan.png"
              alt="Chef"
              class="max-w-[300px] md:max-w-md lg:max-w-lg"
            />
            <div
              class="
                absolute
                -top-10
                -right-16
                drop-shadow-2xl
                z-20
                lg:top-15
                lg:-right-58
                lg:w-[516px]
                md:-top-14
                md:-right-20
              "
            >
              <img
                src="@/assets/images/device.png"
                alt="Celular"
                class="w-full"
              />
            </div>
          </div>
        </div>
      </div>
      <div id="hero-carousel-controls-mobile" class="w-full flex gap-3 justify-center lg:hidden mt-6">
        <img class="user-none self-center cursor-pointer rotate-180" src="@/assets/icons/arrow-hero-alt.svg" alt="slider anterior" />
        <img class="self-center cursor-pointer" src="@/assets/icons/arrow-hero-alt.svg" alt="slider siguiente" />
        <img class="self-center cursor-pointer" src="@/assets/icons/pause-hero.svg" alt="pausar slider" />
      </div>
    </section>
  </section>
</template>

<style scoped>
#hero-carousel {
  background: linear-gradient(
      0deg,
      #3e3cf0,
      #3e3cf0
    ),
    linear-gradient(
      0deg,
      rgba(26, 30, 137, 0.8) 0%,
      rgba(26, 30, 137, 0) 100%
    );
}
</style>
