<script setup lang="ts">
import AppLayout from '@/layouts/AppLayout.vue';
import { type BreadcrumbItem } from '@/types';
import { Head } from '@inertiajs/vue3';
import PlaceholderPattern from '../../components/PlaceholderPattern.vue';

const breadcrumbs: BreadcrumbItem[] = [
    {
        title: 'Home',
        href: '/home',
    },
];
</script>

<template>
    <Head title="Home" />

    <AppLayout :breadcrumbs="breadcrumbs">
        <div class="flex h-full flex-1 flex-col gap-4 rounded-xl p-4">
            <div class="grid grid-cols-3 gap-6">
                <div
                    class="border-sidebar-border/70 dark:border-sidebar-border relative col-span-1 min-h-[100vh] flex-1 rounded-xl border md:min-h-min"
                >
                    <PlaceholderPattern />
                </div>
                <div class="col-span-2 grid auto-rows-min gap-4 md:grid-cols-3">
                    <div class="border-sidebar-border/70 dark:border-sidebar-border relative aspect-video overflow-hidden rounded-xl border">
                        <PlaceholderPattern />
                    </div>
                    <div class="border-sidebar-border/70 dark:border-sidebar-border relative aspect-video overflow-hidden rounded-xl border">
                        <PlaceholderPattern />
                    </div>
                    <div class="border-sidebar-border/70 dark:border-sidebar-border relative aspect-video overflow-hidden rounded-xl border">
                        <PlaceholderPattern />
                    </div>
                </div>
            </div>
        </div>
    </AppLayout>
</template>
