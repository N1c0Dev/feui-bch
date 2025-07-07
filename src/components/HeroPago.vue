<template>
  <section
    id="hero"
    class="
      relative
    "
  >
    <div
      id="hero-message-bar"
      class="
        absolute
        top-0
        left-0
        w-full
        h-12
        z-20
        flex
        gap-4
        items-center
        justify-center
        text-white
        bg-[#1A1E8980]
        px-[var(--section)]
        sm:px-[var(--sm-section)]
      "
    >
      <img
        src="@/assets/icons/truck.svg"
        alt=""
        class="h-6 w-auto"
      />
      <p class="text-sm">
        ¡Contrata hoy y obtén <span class="font-bold">los mejores beneficios</span>!
      </p>
    </div>

  </section>
</template>
<style scoped>
 #hero-carousel {
  background: linear-gradient(0deg, #3E3CF0, #3E3CF0),linear-gradient(0deg, rgba(26, 30, 137, 0.8) 0%, rgba(26, 30, 137, 0) 100%);
 }
 .fan-image {
    border-image-source: linear-gradient(180deg, rgba(52, 51, 209, 0) 77.2%, #3433D1 100%);
 }
 .fan-background {
    background-position: 100%;
    background-position-y: -4rem;
 }
 @keyframes fadeInRight {
  0% {
    opacity: 0;
    transform: translateX(50%);
  }
  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.bg-fade-in-right {
  animation: fadeInRight 1s ease-out forwards;
}
</style>

