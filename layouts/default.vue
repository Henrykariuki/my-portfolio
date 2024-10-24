<script setup>

</script>

<template>
    <div class="flex flex-row gap-2 p-6">
        <div>
            <LeftPanel/>
        </div>
        <div class="grow border border-black p-4">
            <MyHeader />
            <div>
                <slot />
            </div>
        </div>
    </div>
</template>

<style scoped>

</style>