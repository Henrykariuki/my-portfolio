<script setup>
import { Twitter, Linkedin, Instagram, Github, Smartphone, Mail } from 'lucide-vue-next';

const socialIcons = [
    { name: Linkedin, link: 'https://www.linkedin.com/in/henry-kariuki/' },
    { name: Github, link: 'https://github.com/Henrykariuki' },
    { name: Twitter, link: 'https://www.linkedin.com/in/henry-kariuki/' }
]

</script>

<template>
    <div>
        <div class=" md:border-r border-blue-700 md:w-64 px-4 h-full">
            <div class="flex flex-row border-b md:border-hidden border-blue-700 gap-12">
                <div>
                    <img class="w-14 h-14 rounded-full md:w-52 md:h-52 object-cover md:mx-auto md:rounded-lg"
                        src="/images/image.jpg" />
                </div>
                <div class="md:hidden flex flex-col justify-center">
                    <p class="font-semibold">Henry Kariuki</p>
                    <p class="text-xs">Software Developer</p>
                </div>
            </div>
            <div class="hidden md:block my-8">
                <p class="text-xl font-medium">I'm<br><span class="text-5xl font-bold">Henry<br>Kariuki</span></p>
                <p class="my-4">Software Developer</p>
            </div>
            <div class="hidden md:flex flex-col gap-4">
                <div class="flex flex-row gap-2 items-center">
                    <Mail class="text-orange-400" size="17" />
                    <a href="mailto:henrykariuki17@gmail.com">
                        <p class="hover:underline decoration-solid">henrykariuki17@gmail.com</p>
                    </a>
                </div>
                <div class="flex flex-row gap-2 items-center">
                    <Smartphone class="text-orange-400" size="17" />
                    <p>+254713140987</p>
                </div>
            </div>
            <div class="hidden md:flex flex-row gap-4 flex justify-center my-5">
                <div class="hover:scale-95 border border-orange-400 p-1.5 rounded-full text-orange-400" size="15"
                    v-for="(icon, index) in socialIcons" :key="index">
                    <a :href="icon.link" target="_blank">
                        <component :is="icon.name" size="16" />
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

</style>