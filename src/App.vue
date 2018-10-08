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
      <div class="pb-12">
        <h1 class="text-2xl sm:text-3xl text-white font-medium text-center pt-12 pb-16">Start your podcast today:</h1>
        <div class="flex flex-wrap -mx-4">
          <div class="w-full mb-6 md:mb-0 md:w-1/2">
            <plan-selector :schedule="schedule" @change-schedule="schedule = $event" :selected-plan="selectedPlan" @select="selectedPlan = $event"></plan-selector>
          </div>
          <div class="w-full md:w-1/2 px-4 md:pt-10">
            <form action="#" method="POST">
              <h2 class="md:hidden text-center text-white font-medium text-xl mb-4">Your Information</h2>
              <input placeholder="Your Name" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input type="email" placeholder="Your Email" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input type="password" placeholder="Setup Your Password" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <input placeholder="Card number" class="block text-white font-medium text-xl text-center w-full bg-navy-dark focus:bg-navy focus:outline-none px-4 py-4 rounded mb-4">
              <button class="focus:outline-none focus:shadow-outline block w-full bg-yellow uppercase px-4 py-4 font-black text-yellow-dark rounded border-b-2 border-yellow-dark mb-4">Create my account</button>
              <p class="text-white font-bold text-sm text-center">Includes a 14 day trial before billing begins</p>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import PlanSelector from './components/PlanSelector'

  export default {
    name: 'app',
    components: {
      PlanSelector,
    },
    data() {
      return {
        schedule: 'monthly',
        selectedPlan: 'Starter',
      }
    },
  }
</script>

<style>
@tailwind preflight;
@tailwind components;
@tailwind utilities;
</style>
