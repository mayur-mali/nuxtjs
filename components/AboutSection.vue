<template>
  <section
    id="about"
    class="pt-28 pb-32"
    style="background-color:rgba(27,30,50,1)"
  >
    <div class="container mx-auto px-6">
      <div class="flex items-center">
        <div
          class="w-14 h-1 mr-4"
          style="width: 4rem;background-color:rgba(253,67,112,1);"
        >
        </div>
        <p class="font-bold text-white">
          About
        </p>
      </div>
      <div>
        <h2 class="mt-8 lg:text-2.5xl text-4xl font-semibold tracking-wide leading-normal text-white">
          Get a closer look at who I am.
        </h2>
      </div>
      <div class="lg:flex-row lg:mt-30 flex flex-col-reverse items-start mt-16">
        <div class="md:w-7/12 w-full">
          <div class="flex items-center">
            <div
              class="h-1 mr-4"
              style="width: 2.5rem;background-color:rgba(253,67,112,1);"
            >
            </div>
            <p class="font-bold  text-white">
              Who am I
            </p>
          </div>
          <div class="mt-5 leading-9">
            <p class="inline decoration-clone text-white font-semibold px-4 bg-gradient-to-r from-gray-600 to-transparent">
              Developer who thinks about re-usability and readability of code and how extensible is code, how to leverage TDD (Test Driven Development). Working in web domain for more than 6 years and have expert level expertise in Laravel, Vue stack. I am a self taught developer. I know how to find answers and self motivator.
            </p>
          </div>
          <div class="flex items-center mt-5">
            <div
              class="h-1 mr-4"
              style="width: 2.5rem;background-color:rgba(253,67,112,1);"
            >
            </div>
            <p class="font-bold  text-white">
              Skill & Tools
            </p>
          </div>
          <div>
            <div class="mt-5 leading-9">
              <p class="inline decoration-clone text-white font-semibold px-4 bg-gradient-to-r from-gray-600 to-transparent">
                Design: Figma, Photoshop, Illustrator, After Effects
              </p>
            </div>
            <div class="mt-5 leading-9">
              <p class="inline decoration-clone text-white font-semibold px-4 bg-gradient-to-r from-gray-600 to-transparent">
                Development: Laravel, JavaScript, Vue, Nuxt js, Next.js, HTML, CSS/SCSS, TailwindCSS, Node Js
              </p>
            </div>
          </div>
          <div class="md:w-auto flex w-full text-center">
            <a
              href="#work"
              class="bg-indigo-600 mt-10 px-8 py-5 md:w-auto w-full hover:bg-gray-600 font-bold transition duration-700 ease-in-out text-white"
            >Get in touch</a>
          </div>
        </div>
        <div class="md:w-5/12 lg:mb-0 lg:self-start lg:mt-0 flex flex-col justify-center w-9/12 mt-10 mb-10">
          <div style="max-width:100%;width:500px">
            <div
              class="pic"
              style="position:relative;padding-bottom:100%"
            >
              <img
                src="~assets/svg/blob.svg"
                alt="bhushan"
                class="md:max-h-sm md:mt-0 object-contain w-full h-full pointer-events-none"
                style="visibility: visible; height: 100%; left: 0px; position: absolute; top: 0px; width: 100%; margin-top: -50px"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {

};
</script>
<style scoped>

</style>
