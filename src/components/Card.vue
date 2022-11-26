<script setup>
import ListIcon from "./icons/ListIcon.vue";
import TimeIcon from "./icons/TimeIcon.vue";

defineProps({
    msg: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <div class="max-w-lg mx-auto my-10 bg-white p-8 rounded-xl shadow shadow-slate-300">
        <div class="flex flex-row justify-between items-center">
            <div>
                <h1 class="text-3xl font-medium"> {{ msg }} </h1>
            </div>
            <div class="inline-flex space-x-2 items-center">
                <a href="#"
                    class="p-2 border border-slate-200 rounded-md inline-flex space-x-1 items-center text-indigo-200 hover:text-white bg-indigo-600 hover:bg-indigo-500">
                    <TimeIcon />
                </a>
                <a href="#"
                    class="p-2 border border-slate-200 rounded-md inline-flex space-x-1 items-center hover:bg-slate-200">
                    <ListIcon />
                    <span class="text-sm hidden md:block">Latest</span>
                </a>
            </div>
        </div>
        <p class="text-slate-500">Hello, here are your latest tasks</p>
    </div>
</template>

<style scoped>

</style>
