<script setup>

const projectNames = [
    { name: 'SokoMax', image: '/images/sokomax.jpg', link: 'https://dashboard-iq.vercel.app' },
    { name: 'Dashboard-Iq', image: '/images/dashboardiq.jpg', link: 'https://dashboard-iq.vercel.app' },
    { name: 'Launch Mart', image: '/images/launchmart.jpg', link: 'https://launch-mart.vercel.app' },
    { name: 'Watches Online Store', image: '/images/henrywatches.jpg', link: 'https://watches-online-store.vercel.app'},
]
</script>
<template>
    <div>
        <p class="font-bold text-3xl">Projects</p>
        <div class="grid md:grid-cols-2 gap-6 pt-5">
            <ProjectsCard v-for="(project, index) in projectNames" :key="`id${index}`" :name="project" />
        </div>
    </div>
</template>

<style scoped></style>