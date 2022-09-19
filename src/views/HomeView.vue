<template>
  <div>
    <div
      class="
        absolute
        -z-20
        top-0
        inset-x-0
        flex
        justify-center
        overflow-hidden
        pointer-events-none
      "
    >
      <div class="w-[100%] flex-none flex justify-end">
        <picture>
          <source
            srcset="
              ../assets/light.avif
            "
            type="image/avif"
          />
          <img
            src="../assets/light.jpeg"
            alt=""
            class="w-[90rem] flex-none max-w-none dark:hidden"
            decoding="async"
          />
        </picture>
        <picture>
          <source
            srcset="
              ../assets/dark.avif
            "
            type="image/avif"
          />
          <img
            src="../assets/dark.jpg"
            alt=""
            class="w-[90rem] flex-none max-w-none hidden dark:block"
            decoding="async"
          />
        </picture>
      </div>
    </div>
    <div
      class="
        w-full
        fixed
        inset-0
        bg-slate-100/40
        backdrop-blur-md
        dark:bg-black/40 shadow-lg
      "
    >
      <div
        class="
          top-1/2
          left-1/2
          right-1/2
          transform
          fixed
          w-full
          -translate-y-1/2 -translate-x-1/2
        "
      >
        <img
          src="../assets/loadind.png"
          srcset="../assets/loadind.png 2x"
          alt=""
          class="w-1/3 h-1/3 lg:w-1/4 mx-auto lg:h-1/4 animate-bounce animate"
        />
      </div>
    </div>
    <div class="hidden"></div>
  </div>
</template>
