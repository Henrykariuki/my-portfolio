<script setup>
const buttons = [
    { name: 'About', route: '/about' },
    { name: 'Projects', route: '/projects' },
    { name: 'Resume', route: '/Resume' },
]
</script>

<template>
    <div>
        <div class="flex justify-around text-white border-b border-blue-700 font-semibold pb-4 mb-4">
            <nav v-for="(nav, index) in buttons" :key="`id-${index}`">
                <NuxtLink class="hover:text-blue-200" :to="nav.route">{{ nav.name }}</NuxtLink>
            </nav>
        </div>
    </div>
</template>

<style scoped>

</style>