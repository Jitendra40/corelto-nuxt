<script setup lang="ts">
import { Button } from '@/components/ui/button'
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from '@/components/ui/card'
</script>
<template>
    <div class="flex items-center justify-center banner-height ">
        <div class="text-center">
            <span class="bg-brand text-white rounded-full p-1 px-3 text-xs leading-none mb-2 inline-flex">CRM Made Easy</span>
            <h1 class="text-xl md:text-4xl lg:text-6xl font-bold mb-4 bg-gradient-to-r from-brand to-brand-light text-transparent bg-clip-text">Unleash the Power of Real Estate CRM</h1>
            <h3 class="text-lg md:text-xl lg:text-4xl font-bold mb-4">Technology that transforms your Business</h3>
            <p class="text-lg font-normal text-gray-800 max-w-2xl text-center m-auto mb-5">CRM software provides a centralized database where businesses can store and manage customer information
                and many more...</p>
            <Button class="bg-brand hover:bg-orange-500 text-lg font-normal p-6">Request a demo</Button>
        </div>
    </div>
</template>