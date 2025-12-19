<template>
  <div :class="boxClasses">
    <slot />
  </div>
</template>

<script setup>
const props = defineProps({
  color: {
    type: String,
    default: 'red'
  }
})

const colorMap = {
  red: 'border-red-500 bg-red-50',
  blue: 'border-blue-500 bg-blue-50',
  green: 'border-green-500 bg-green-50',
  yellow: 'border-yellow-500 bg-yellow-50',
  orange: 'border-orange-500 bg-orange-50',
  purple: 'border-purple-500 bg-purple-50',
  pink: 'border-pink-500 bg-pink-50',
  indigo: 'border-indigo-500 bg-indigo-50',
  teal: 'border-teal-500 bg-teal-50',
  cyan: 'border-cyan-500 bg-cyan-50',
  gray: 'border-gray-500 bg-gray-50',
  slate: 'border-slate-500 bg-slate-50',
  emerald: 'border-emerald-500 bg-emerald-50',
  lime: 'border-lime-500 bg-lime-50',
  amber: 'border-amber-500 bg-amber-50'
}

const boxClasses = `border-2 rounded-lg px-4 pb-2 pt-0 ${colorMap[props.color] || colorMap.red}`
</script>