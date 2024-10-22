<script setup>

</script>

<template>
    <div class="flex flex-row gap-2">
        <div>
            <LeftPanel/>
        </div>
        <div class="grow border border-black">
            <MyHeader />
            <div>
                <slot />
            </div>
        </div>
    </div>
</template>

<style scoped>

</style>