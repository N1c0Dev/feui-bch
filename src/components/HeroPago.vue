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
        bg-[#1A1E8980]
      "
    >
      <img
        src="@/assets/icons/truck.svg"
        alt=""
        class="w-[30px] h-[18px]"
      />
      <p
        class="
          text-sm
          leading-6
          lg:text-xl
        "
      >
        ¡Contrata hoy y obtén <span class="font-bold">los mejores beneficios</span>!
      </p>
    </div>
    <section
      id="hero-carousel"
      class="
        pt-14
        rounded-b-[56px]
      "
    >
      <div
        id="hero-carousel-sliders"
        class="
          flex
          w-full
        "
      >
        <div
          class="
            w-1/2
            flex
          "
        >
          <div
            class="
              m-auto
              lg:max-w-[465px]
              lg:my-20
            "
          >
            <h2
              class="
                text-white
                font-light
                leading-12
                lg:text-[40px]
              "
            >
              Hazte cliente empresa del Banco de Chile <span class="font-bold">y obtén tu producto a costo $0*</span>
            </h2>
            <div
              class="
                flex
                gap-6
                mt-10
              "
            >
              <button
                class="
                  py-4
                  px-6
                  bg-btn-fill
                  text-btn-fill-text
                  font-bold
                  text-sm
                  leading-6
                  text-center
                  uppercase
                  rounded-full
                  cursor-pointer
                  lg:w-[198px]
                "
              >
                <p>
                  QUIERO CONTRATAR
                </p>
              </button>
              <button
                class="
                  py-4
                  px-6
                  bg-transparent
                  text-white
                  font-bold
                  text-sm
                  leading-6
                  text-center
                  uppercase
                  rounded-full
                  border-2
                  cursor-pointer
                  lg:w-[206px]
                "
              >
                <p>
                  Nuestras tarifas
                </p>
              </button>
            </div>
            <div
              id="hero-carousel-controls-mobile"
              class="
                w-full
                hidden
                gap-3
                mt-15
                lg:flex
              "
            >
              <img class="user-none self-center cursor-pointer rotate-180" src="@/assets/icons/arrow-hero-alt.svg" alt="slider anterior">
              <img class="self-center cursor-pointer" src="@/assets/icons/arrow-hero-alt.svg" alt="slider siguiente">
              <img class="self-center cursor-pointer" src="@/assets/icons/pause-hero.svg" alt="pausar slider">
            </div>
          </div>
        </div>
        <div class="w-1/2">B</div>
      </div>
      <div
        id="hero-carousel-controls-mobile"
        class="
          w-full
          flex
          gap-3
          justify-center
          lg:hidden
        "
      >
        <img class="user-none self-center cursor-pointer rotate-180" src="@/assets/icons/arrow-hero-alt.svg" alt="slider anterior">
        <img class="self-center cursor-pointer" src="@/assets/icons/arrow-hero-alt.svg" alt="slider siguiente">
        <img class="self-center cursor-pointer" src="@/assets/icons/pause-hero.svg" alt="pausar slider">
      </div>
    </section>
  </section>
</template>
<style scoped>
 #hero-carousel {
  background: linear-gradient(0deg, #3E3CF0, #3E3CF0),linear-gradient(0deg, rgba(26, 30, 137, 0.8) 0%, rgba(26, 30, 137, 0) 100%);
}
</style>

