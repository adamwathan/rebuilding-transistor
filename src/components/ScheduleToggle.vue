<template>
  <div class="w-40 bg-navy-dark mx-auto flex rounded mb-4">
    <button type="button" @click="select('monthly')"
      class="focus:outline-none focus:shadow-outline rounded py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide"
      :class="[isMonthly ? 'bg-white text-navy-darker ' : 'text-navy-light hover:text-white hover:bg-navy']"
    >
      Monthly
    </button>
    <button type="button" @click="select('yearly')"
      class="focus:outline-none focus:shadow-outline rounded py-1 uppercase text-center w-1/2 text-xs font-bold tracking-wide"
      :class="[isYearly ? 'bg-white text-navy-darker ' : 'text-navy-light hover:text-white hover:bg-navy']"
    >
      Yearly
    </button>
  </div>
</template>

<script>
  export default {
    props: ['value'],
    computed: {
      isMonthly() {
        return this.value === 'monthly'
      },
      isYearly() {
        return this.value === 'yearly'
      }
    },
    methods: {
      select(schedule) {
        this.$emit('input', schedule)
      }
    },
  }
</script>
