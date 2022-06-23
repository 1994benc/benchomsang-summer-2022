<template>
  <div class="container">
    <h1 class="text-7xl">Let's talk</h1>

    <div class="my-8 space-y-6">
      <form class="flex flex-col gap-4">
        <input class="form" type="text" placeholder="Your name" >
        <input class="form" type="text" placeholder="Email address" >
        <textarea class="form" placeholder="Your message" cols="30" rows="10">
        </textarea>
      </form>

      <ComingSoonMessage message="This form is still under construction 🚧 Please email 1994benc@gmail.com." />

      <!-- <div class="flex gap-3 items-center">
        <button class="button">Send</button>
        <small>I will get back to you as soon as possible</small>
      </div> -->
    </div>
  </div>
</template>
