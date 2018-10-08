<template>
  <div id="app" class="min-h-screen bg-navy-darker font-sans antialiased leading-tight">
    <div class="container mx-auto px-6">
      <header class="flex justify-between items-center py-8">
        <div>
          <img class="block h-12" src="./assets/transistor-logo.svg" alt="Transistor">
        </div>
        <div>
          <a href="#" class="font-medium no-underline text-white hover:underline">Sign In</a>
        </div>
      </header>
      <div class="">
        <h1 class="text-white font-medium text-center pt-12 pb-16">Start your podcast today:</h1>
        <div class="flex flex-wrap -mx-4">
          <div class="w-1/2 px-4 pt-10 relative">
            <div class="absolute pin-x pin-t">
              <div class="w-40 bg-navy-dark text-navy-light mx-auto flex rounded overflow-hidden mb-4">
                <span class="rounded bg-white text-navy-darker py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide">Monthly</span>
                <span class="rounded py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide hover:text-white hover:bg-navy">Yearly</span>
              </div>
            </div>
            <div class="border border-navy-dark bg-navy-dark rounded px-6 py-4 mb-4 relative">
              <div class="absolute pin-l pin-y flex items-center">
                <svg class="h-8 w-8 -ml-4" version="1.1" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                  <path d="M20.49,3.51l-9.98275e-08,-9.94815e-08c-4.69442,-4.67815 -12.2924,-4.66496 -16.9705,0.029463c-4.67815,4.69442 -4.66496,12.2924 0.029463,16.9705c4.6829,4.66667 12.2582,4.66667 16.9411,-1.98963e-07l-1.99655e-07,1.98963e-07c4.69442,-4.67815 4.70761,-12.2761 0.029463,-16.9705c-0.00980385,-0.00983795 -0.0196248,-0.0196589 -0.0294627,-0.0294627Zm-2.73,5.14l-6.61,7.71l-4.75,-3.56l-6.60367e-08,-4.95276e-08c-0.441828,-0.331371 -0.531371,-0.958172 -0.2,-1.4c0.331371,-0.441828 0.958172,-0.531371 1.4,-0.2l3.25,2.44l5.39,-6.29l-3.71146e-08,4.33955e-08c0.358985,-0.419736 0.990264,-0.468985 1.41,-0.11c0.419736,0.358985 0.468985,0.990264 0.11,1.41Z" fill="#FFF"></path>
                </svg>
              </div>
              <div class="flex items-center -mx-4">
                <div class="px-4 w-2/5 text-white">
                  <h2 class="text-lg font-medium mb-2">Starter</h2>
                  <div class="font-medium">
                    <span class="text-3xl font-bold">$19</span>
                    <span class="mx-1">/</span>
                    <span>month</span>
                  </div>
                </div>
                <div class="px-4 w-3/5">
                  <ul class="list-reset text-sm text-navy-lighter font-medium">
                    <li class="mb-1">5,000 downloads / month</li>
                    <li class="mb-1">Unlimited shows and episodes</li>
                    <li>Analytics, teams, and more…</li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="border border-navy-dark rounded px-6 py-4 mb-4 opacity-50 hover:opacity-100 hover:bg-navy-dark">
              <div class="flex items-center -mx-4">
                <div class="px-4 w-2/5 text-white">
                  <h2 class="text-lg font-medium mb-2">Professional</h2>
                  <div class="font-medium">
                    <span class="text-3xl font-bold">$49</span>
                    <span class="mx-1">/</span>
                    <span>month</span>
                  </div>
                </div>
                <div class="px-4 w-3/5">
                  <ul class="list-reset text-sm text-navy-lighter font-medium">
                    <li class="mb-1">15,000 downloads / month</li>
                    <li class="mb-1">Unlimited shows and episodes</li>
                    <li>Analytics, teams, and more…</li>
                  </ul>
                </div>
              </div>
            </div>
            <div class="border border-navy-dark rounded px-6 py-4 opacity-50 hover:opacity-100 hover:bg-navy-dark">
              <div class="flex items-center -mx-4">
                <div class="px-4 w-2/5 text-white">
                  <h2 class="text-lg font-medium mb-2">Small Business</h2>
                  <div class="font-medium">
                    <span class="text-3xl font-bold">$99</span>
                    <span class="mx-1">/</span>
                    <span>month</span>
                  </div>
                </div>
                <div class="px-4 w-3/5">
                  <ul class="list-reset text-sm text-navy-lighter font-medium">
                    <li class="mb-1">45,000 downloads / month</li>
                    <li class="mb-1">Unlimited shows and episodes</li>
                    <li>Analytics, teams, and more…</li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="w-1/2 px-4 pt-10">
            <form action="#" method="POST" class="">
              <input placeholder="Your Name" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input type="email" placeholder="Your Email" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input type="password" placeholder="Setup Your Password" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input placeholder="Card number" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <button class="block w-full bg-yellow uppercase px-4 py-4 font-black text-yellow-dark rounded border-b-2 border-yellow-dark mb-4">Create my account</button>
              <p class="text-white font-bold text-sm text-center">Includes a 14 day trial before billing begins</p>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'app',
  components: {
  }
}
</script>

<style>
@tailwind preflight;
@tailwind components;
@tailwind utilities;
</style>
