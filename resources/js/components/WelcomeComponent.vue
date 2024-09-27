<template>
    <div class="grid gap-12 lg:grid-cols-12 lg:gap-12">
        <a href="https://laracasts.com" class="flex items-start gap-12 rounded-lg bg-white p-6 shadow-[0px_14px_34px_0px_rgba(0,0,0,0.08)] ring-1 ring-white/[0.05] transition duration-300 hover:text-black/70 hover:ring-black/20 focus:outline-none focus-visible:ring-[#FF2D20] lg:pb-10 dark:bg-zinc-900 dark:ring-zinc-800 dark:hover:text-white/70 dark:hover:ring-zinc-700 dark:focus-visible:ring-[#FF2D20]">
            <div class="pt-3 sm:pt-5">
                <h2 class="text-xl font-semibold text-black dark:text-white">Welcome to Laravel 11 & vue js 3</h2>
                <p class="mt-4 text-sm/relaxed">
                    <span v-bind:style="{ color: titleColor }">{{ title1 }}</span><br>
                    {{ content1 }}
                </p>
                <p class="mt-4 text-sm/relaxed">  
                    <span :style="{color: titleColor}">{{title2}}</span><br>
                    {{ content12 }}
                </p>
            </div>           
        </a>
    </div>
</template>
<script>
export default{
    data() {
        return {
            titleColor: "#FF2D20",
            title1: "Features of Laravel 11",
            content1: `Vite Integration: Laravel 11 uses Vite for fast builds and hot reloading.
                    Improved Performance: Laravel 11 introduces faster query processing and task scheduling improvements.
                    New Query Builder: More streamlined and efficient query handling.
                    Advanced Queueing System: Enhancements in job queues and background tasks.
                    Improved Exception Handling: More detailed error messages and stack traces for debugging.
                    Security Updates: Stronger encryption algorithms and improved authentication features.
                    PHP 8.2 Support: Laravel 11 is fully compatible with the latest PHP versions, providing access to new language features.`,
            title2: "Features of Vue.js 3",
            content12 : `Composition API: A new flexible and scalable way of organizing components, allowing for better code reuse.
                    Teleport: A feature that allows components to be rendered outside their parent DOM tree.
                    Fragments: Vue 3 allows multiple root elements in components, providing more flexibility.
                    Suspense: Built-in async handling for better control over asynchronous component loading.
                    Improved Performance: Vue 3 is faster and more efficient than Vue 2 due to its rewritten reactivity system and tree-shaking abilities.
                    TypeScript Support: Vue 3 has built-in TypeScript support for better type safety and tooling integration.`,
        }
    },
}
</script>