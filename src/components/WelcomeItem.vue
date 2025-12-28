<template>
  <div class="mt-8 flex relative lg:mt-0 lg:py-1.5 lg:pb-4 lg:pr-0 lg:pl-[calc(var(--section-gap)/2)] before:content-[''] before:border-l before:border-[var(--color-border)] before:absolute before:left-0 before:bottom-[calc(50%+25px)] before:h-[calc(50%-25px)] before:lg:block before:hidden after:content-[''] after:border-l after:border-[var(--color-border)] after:absolute after:left-0 after:top-[calc(50%+25px)] after:h-[calc(50%-25px)] after:lg:block after:hidden first:before:hidden last:after:hidden">
    <i class="flex items-center justify-center w-8 h-8 text-[var(--color-text)] lg:top-[calc(50%-25px)] lg:-left-[26px] lg:absolute lg:border lg:border-[var(--color-border)] lg:bg-[var(--color-background)] lg:rounded-lg lg:w-[50px] lg:h-[50px]">
      <slot name="icon"></slot>
    </i>
    <div class="flex-1 ml-4">
      <h3 class="text-xl font-medium mb-1.5 text-[var(--color-heading)]">
        <slot name="heading"></slot>
      </h3>
      <slot></slot>
    </div>
  </div>
</template>
