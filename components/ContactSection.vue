<template>
  <section
    id="contact"
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
          Contact
        </p>
      </div>
      <div>
        <h2 class="mt-8 lg:text-2.5xl text-4xl font-semibold tracking-wide leading-normal text-white">
          Interested in working with me
        </h2>
      </div>
      <div>
        <p class="md:w-3/5 lg:w-1/3 connect-content text-gray-400 w-full mt-6 text-base font-normal leading-loose">
          Reach me on social media, by filling out the contact form or by sending an email to <a
            href="mailto:bhushangaykawad@gmail.com"
            class="font-bold text-sm text-pink-700"
          >
            bhushangaykawad@gmail.com
          </a>
        </p>
      </div>
      <div id="form_wrapper">
        <div class="md:w-5/5 lg:w-2/5 w-full mt-20">
          <div class="flex flex-col space-y-8">
            <div>
              <label
                for="name"
                class="flex flex-col text-white"
              >
                What’s your name?
                <input
                  id="name"
                  type="text"
                  class="focus:outline-none py-3 mt-3 text-white px-4 border-l-4 border-indigo-600 bg-gray-900"
                />
              </label>
            </div>
            <div>
              <label
                for="email"
                class="flex flex-col text-white"
              >
                Your email address
                <input
                  id="email"
                  type="email"
                  class="focus:outline-none py-3 mt-3 text-white px-4 border-l-4 border-indigo-600 bg-gray-900"
                />
              </label>
            </div>
            <div>
              <label
                for="textarea"
                class="flex flex-col text-white"
              >
                Type your message here
                <textarea
                  id="textarea"
                  v-model="message"
                  maxlength="142"
                  class="focus:outline-none h-32 py-3 my-3 text-white px-4 border-l-4 border-indigo-600 bg-gray-900"
                  @keyup="remaincharCount()"
                > </textarea>
              </label>
              <span class="text-white font-bold tracking-wider">
                {{ remaincharactersText }}
              </span>
              <div>
                <span
                  v-if="message.length <= 10 && message.length >= 1"
                  class="text-white font-bold tracking-wider"
                >
                  Your message requires a length of 10 characters.
                </span>
              </div>
            </div>
            <div
              v-if="message.length >= 1"
              class="md:w-auto flex w-full text-center"
            >
              <a
                href="#work"
                class="bg-indigo-600 mt-5 px-8 py-5 md:w-auto w-full hover:bg-gray-600 font-bold transition duration-700 ease-in-out text-white"
              >Sent a massage</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      message: '',
      maxcharacter: 140,
      mincharacter: 10,
      error: '',
      remaincharactersText: '0 / 140',
    };
  },
  methods: {
    remaincharCount () {
      if (this.message.length > this.maxcharacter) {
        this.remaincharactersText = 'meet max length';
      } else {
        const remainCharacters = this.maxcharacter - this.message.length;
        this.remaincharactersText = remainCharacters + ' / 140';
      }
    },
  },

};
</script>
<style scoped>

</style>
