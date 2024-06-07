<script setup>
import { ref } from 'vue';
import MainLayout from '@/Layouts/MainLayout.vue';
import { Head } from '@inertiajs/vue3';

const posts = ref(10);
</script>

<template>
    <Head title="Inicio" />

    <MainLayout>
        <div class="py-12">
            <div class="flex flex-col gap-4">
                <div v-for="post in posts" class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                    <div class="bg-white dark:bg-gray-800 overflow-hidden shadow-sm sm:rounded-lg">
                        <div class="flex gap-2 align-middle px-6 pt-6 text-gray-900 dark:text-gray-100">
                            <span class="bg-gray-200 p-2 px-3 align-middle text-center rounded-full">
                                (foto usuario)
                            </span>
                            <span class="p-2">
                                Arthur Tachini
                            </span>
                        </div>
                        <div class="p-6 text-gray-900 dark:text-gray-100">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores aspernatur, quisquam odit fuga ipsum facere enim iste error omnis saepe voluptas repudiandae officiis rem ab quod, sed cumque, incidunt ut.</div>
                    </div>
                </div>
            </div>
        </div>
    </MainLayout>
</template>
