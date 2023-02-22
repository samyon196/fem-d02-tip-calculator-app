<script setup>
import IconMoon from '~icons/carbon/moon'
import IconSun from '~icons/carbon/sun'
import { useDark, useToggle } from '@vueuse/core'
const isDark = useDark()
const toggleDark = useToggle(isDark)
</script>

<template>
    <div
        v-auto-animate
        class="bg-gray-300 w-12 h-12 flex items-center justify-center rounded-1/2 shadow-xl m-4"
        @click="toggleDark()"
    >
        <icon-moon v-if="isDark" class="text-3xl text-purple-500" />
        <icon-sun v-else class="text-3xl text-yellow-500" />
    </div>
</template>
