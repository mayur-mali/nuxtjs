<template>
  <div
    class="w-full fixed z-50"
    :class="{ classA: scrollPosition < 100, classB: scrollPosition > 100 }"
  >
    <nav
      class="container px-10 mx-auto"
    >
      <div class="flex justify-between items-center">
        <div>
          <img
            src="~/assets/svg/logonav.svg"
            alt="logonav"
            class="h-20 hidden w-20"
          />
        </div>
        <div class="space-x-8">
          <a
            href="#work"
            class="text-gray-300 font-bold"
          >Work</a>
          <a
            href="#about"
            class="text-gray-300 font-bold"
          >About</a>
          <a
            href="#contact"
            class="text-gray-300 font-bold"
          >Contact</a>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data () {
    return {
      scrollPosition: null,
    };
  },

  mounted () {
    window.addEventListener('scroll', this.updateScroll);
  },
  methods: {
    updateScroll () {
      this.scrollPosition = window.scrollY;
    },
  },
};
</script>
<style scoped>
.classA {
  background-color: rgba(20,22,40,1);
  padding: 3rem 0;
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
  -webkit-transition-duration: 200ms;
  -o-transition-duration: 200ms;
  transition-duration: 200ms;
  -webkit-transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  -o-transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}
.classB {
  width: 100%;
  padding: 1.5rem 0;
    background-color: rgba(20,22,40,1);
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
  -webkit-transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  -o-transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  -webkit-transition-duration: 200ms;
  -o-transition-duration: 200ms;
  transition-duration: 200ms;
}
</style>
