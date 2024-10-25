<script setup>
import { Twitter, Linkedin, Instagram, Github, Smartphone, Mail } from 'lucide-vue-next';
const socialIcons = [
    { name: Linkedin, link: 'https://www.linkedin.com/in/henry-kariuki/' },
    { name: Github, link: 'https://github.com/Henrykariuki' },
    { name: Twitter, link: 'https://www.linkedin.com/in/henry-kariuki/' }
]
</script>

<template>
    <div class="md:hidden flex flex-col items-center bg-black text-white py-6 mt-2">
        <div class="flex items-center flex-col gap-4">
            <div class="flex flex-row gap-1 items-center">
                <Mail class="text-orange-400" size="17" />
                <a href="mailto:henrykariuki17@gmail.com">
                    <p class="hover:underline decoration-solid">henrykariuki17@gmail.com</p>
                </a>
            </div>
            <div class="flex flex-row gap-1 items-center">
                <Smartphone class="text-orange-400" size="17" />
                <p>+254713140987</p>
            </div>
        </div>
        <div class="flex flex-row gap-4  mt-8">
            <div class="hover:scale-95 border border-orange-400 p-1.5 rounded-full text-orange-400" size="15"
                v-for="(icon, index) in socialIcons" :key="index">
                <a :href="icon.link" target="_blank">
                    <component :is="icon.name" size="16" />
                </a>
            </div>
        </div>
    </div>
</template>

<style scoped>

</style>