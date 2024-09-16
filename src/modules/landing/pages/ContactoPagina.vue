<template>
  <!-- <h1 class="text-3xl font-bold underline">Contacto</h1> -->
  <!-- component -->
  <!-- <section> -->
  <div class="relative map-container">
    <iframe
      width="100%"
      height="100%"
      frameborder="0"
      marginheight="0"
      marginwidth="0"
      title="map"
      scrolling="no"
      src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d3876.713421186518!2d-89.194147!3d13.675182!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8f63311954327075%3A0x28682274f5650dd1!2sUniversidad%20Luterana%20Salvadore%C3%B1a!5e0!3m2!1ses!2ssv!4v1726455487078!5m2!1ses!2ssv"
    ></iframe>
  </div>
  <!-- <div class="container px-5 py-24 mx-auto flex"> -->
  <div
    class="absolute bottom-20 right-10 m-8 sm:w-full md:w-1/2 lg:w-1/5 bg-white rounded-lg p-8 flex flex-col max-w-sm z-10 shadow-lg"
  >
    <h2 class="text-gray-900 text-lg mb-1 font-medium title-font">Feedback</h2>
    <p class="leading-relaxed mb-5 text-gray-600">
      Post-ironic portland shabby chic echo park, banjo fashion axe
    </p>
    <div class="relative mb-4">
      <label for="email" class="leading-7 text-sm text-gray-600">Email</label>
      <input
        type="email"
        id="email"
        name="email"
        class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out"
      />
    </div>
    <div class="relative mb-4">
      <label for="message" class="leading-7 text-sm text-gray-600">Message</label>
      <textarea
        id="message"
        name="message"
        class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out"
      ></textarea>
    </div>
    <button
      class="text-white bg-indigo-500 border-0 py-2 px-6 focus:outline-none hover:bg-indigo-600 rounded text-lg"
    >
      Button
    </button>
    <p class="text-xs text-gray-500 mt-3">
      Chicharrones blog helvetica normcore iceland tousled brook viral artisan.
    </p>
  </div>
  <!-- </div> -->
  <!-- </section> -->
</template>
<style scoped>
.map-container {
  height: 77vh;
  width: 98vw;
  position: relative;
}
</style>
