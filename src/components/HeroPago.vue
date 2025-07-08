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
        class="
          w-[30px]
          h-[18px]
        "
      />
      <p
        class="
          text-sm
          leading-6
          bg-transparent
          lg:text-xl
        "
      >
        ¡Contrata hoy y obtén <span class="font-bold">los mejores beneficios</span>!
      </p>
    </div>
    <section
      id="hero-carousel"
      class="rounded-b-[56px]"
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
              max-w-[300px]
              mt-25
              text-center
              lg:max-w-[465px]
              lg:text-left
              lg:mt-35
              lg:mb-20
              "
            >
            <h2
              class="
                text-white
                font-light
                text-3xl
                leading-10
                lg:text-[40px]
                lg:leading-12
              "
            >
              Hazte cliente empresa del Banco de Chile
              <span class="font-bold">y obtén tu producto a costo $0*</span>
            </h2>
            <div
              class="
                flex
                flex-col
                gap-6
                mt-10
                lg:flex-row
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
                <p>QUIERO CONTRATAR</p>
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
                <p>Nuestras tarifas</p>
              </button>
            </div>
            <div
              id="hero-carousel-controls-desktop"
              class="
                w-full
                hidden
                gap-3
                mt-15
                lg:flex
              "
            >
              <img
                class="
                  self-center
                  cursor-pointer
                  rotate-180
                "
                src="@/assets/icons/arrow-hero-alt.svg"
                alt="slider anterior"
              />
              <img
                class="
                  self-center
                  cursor-pointer
                "
                src="@/assets/icons/arrow-hero-alt.svg"
                alt="slider siguiente"
              />
              <img
                class="
                  self-center
                  cursor-pointer
                "
                src="@/assets/icons/pause-hero.svg"
                alt="pausar slider"
              />
            </div>
          </div>
        </div>
        <div
          class="
            w-1/2
            relative
            flex
            items-center
            overflow-hidden
          "
        >
          <img
            src="@/assets/images/bg-shape.svg"
            alt=""
            class="
              absolute
              opacity-80
              z-0
              pointer-events-none
              rotate-[0deg]
              md:top-[-80px]
              md:right-[-60px]
              lg:top-[-100px]
              lg:right-[-120px]
              lg:w-[687px]
              lg:h-[635px]
              xl:right-[-50px]
              2xl:right-[-65px]
              2xl:w-[900px]
              2xl:h-[632px]
            "
          />
          <div
            class="
              relative
              z-10
              mt-[100px]
              lg:mt-15
            "
          >
            <img
              class="
                hidden
                lg:max-w-lg
                lg:block
                animate-fade-in-up
              "
              src="@/assets/images/person-fan.png"
              alt=""
            />
            <img
              class="
                md:w-[313px]
                lg:hidden
                animate-fade-in-up-
              "
              src="@/assets/images/person-fan-mobile.png"
              alt=""
            />
            <div
              class="
                absolute
                -top-10
                -right-16
                drop-shadow-2xl
                z-20
                md:top-12
                md:-right-30
                md:w-[310px]
                lg:top-15
                lg:-right-58
                lg:w-[516px]
                animate-fade-in-right
                animate-float
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
      <div
        id="hero-carousel-controls-mobile"
        class="
          w-full
          py-8
          flex
          gap-3
          justify-center
          lg:hidden
        "
      >
        <img
          class="
            self-center
            cursor-pointer
            rotate-180
          "
          src="@/assets/icons/arrow-hero-alt.svg"
          alt="slider anterior"
        />
        <img
          class="
            self-center
            cursor-pointer
          "
          src="@/assets/icons/arrow-hero-alt.svg"
          alt="slider siguiente"
        />
        <img
          class="
            self-center
            cursor-pointer
          "
          src="@/assets/icons/pause-hero.svg"
          alt="pausar slider"
        />
      </div>
    </section>
  </section>
</template>

<style scoped>
#hero-carousel {
  background:
    linear-gradient(
      0deg,
       #201ea9,
       #3433D1
    ),
    linear-gradient(
      0deg,
      rgba(26, 30, 137, 0.8) 0%,
      rgba(26, 30, 137, 0) 100%
    );
}

@keyframes fade-in-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}
@keyframes fade-in-right {
  0% {
    opacity: 0;
    transform: translateX(20px);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}
@keyframes float {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}
.animate-fade-in-up {
  animation: fade-in-up 0.8s ease-out both;
}
.animate-fade-in-right {
  animation: fade-in-right 0.8s ease-out both;
}
.animate-float {
  animation: float 5s ease-in-out infinite;
}
</style>


border-bottom: 72px solid;

border-image-source: linear-gradient(180deg, rgba(52, 51, 209, 0) 77.2%, #2829AF 100%);

