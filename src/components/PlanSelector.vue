<template>
  <div class="px-4 pt-10 relative">
    <div class="absolute pin-x pin-t">
      <schedule-toggle :value="schedule" @input="$emit('change-schedule', $event)"></schedule-toggle>
    </div>
    <plan-card @select="selectPlan('Starter')" :schedule="schedule" name="Starter" monthly="19" yearly="190" :selected="selectedPlan === 'Starter'" :features="[
      '5,000 downloads / month',
      'Unlimited shows and episodes',
      'Analytics, teams, and more…',
    ]"></plan-card>
    <plan-card @select="selectPlan('Professional')" :schedule="schedule" name="Professional" monthly="49" yearly="490" :selected="selectedPlan === 'Professional'" :features="[
      '15,000 downloads / month',
      'Unlimited shows and episodes',
      'Analytics, teams, and more…',
    ]"></plan-card>
    <plan-card @select="selectPlan('Small Business')" :schedule="schedule" name="Small Business" monthly="99" yearly="990" :selected="selectedPlan === 'Small Business'" :features="[
      '45,000 downloads / month',
      'Unlimited shows and episodes',
      'Analytics, teams, and more…',
    ]"></plan-card>
  </div>
</template>

<script>
  import PlanCard from './PlanCard'
  import ScheduleToggle from './ScheduleToggle'

  export default {
    components: {
      PlanCard,
      ScheduleToggle,
    },
    props: [
      'schedule',
      'selectedPlan',
    ],
    methods: {
      selectPlan(plan) {
        this.$emit('select', plan)
      }
    },
  }
</script>
