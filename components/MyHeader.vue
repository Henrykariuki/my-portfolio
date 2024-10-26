<script setup>
const buttons = [
    { name: 'About', route: '/' },
    { name: 'Projects', route: '/projects' },
    { name: 'Resume', route: '/Resume' },
]
</script>

<template>
    <div>
        <div class="flex justify-between mb-4 p-4 md:justify-around text-white md:border-b border-blue-700 md:font-semibold md:pb-4 md:mb-4">
            <nav v-for="(nav, index) in buttons" :key="`id-${index}`">
                <NuxtLink class="hover:text-blue-200" :to="nav.route" active-class="text-blue-200">{{ nav.name }}</NuxtLink>
            </nav>
        </div>
    </div>
</template>

<style scoped>

</style>