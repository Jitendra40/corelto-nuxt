<script setup lang="ts">
import { Carousel, CarouselContent, CarouselItem, CarouselNext, CarouselPrevious } from '@/components/ui/carousel'
</script>
<template>
    <div class=" bg-banner p-4 md:p-16 lg:p-20 xl:p-24">
        <div class="xl:container">
            <div class="text-center">
                <h2 class="text-xl md:text-2xl lg:text-4xl font-bold mb-4 text-black">What our clients say?</h2>
                <p class="text-lg font-normal text-gray-800 max-w-xl text-center m-auto mb-12">Trusted by millions of
                    customers across the world</p>
            </div>
            <Carousel class="relative w-full max-w-4xl mx-auto">
                <CarouselContent>
                    <CarouselItem>
                        <blockquote class="px-6">
                            <p class="text-lg font-normal text-gray-800  mb-8 ">Completely drive innovative value
                                reinvent prospective whereas out-of-the-box paradigms. Interactively pursue stand-alone
                                markets after global say that they results. Professionally metrics expedite</p>
                            <footer class="mt-4 text-sm font-medium text-gray-700 sm:mt-6">
                                &mdash; Global group | Aakash N | Mumbai India
                            </footer>
                        </blockquote>
                    </CarouselItem>
                    <CarouselItem>
                        <blockquote class="px-6">
                            <p class="text-lg font-normal text-gray-800  mb-8 ">Completely drive innovative value
                                reinvent prospective whereas out-of-the-box paradigms. Interactively pursue stand-alone
                                markets after global say that they results. Professionally metrics expedite</p>
                            <footer class="mt-4 text-sm font-medium text-gray-700 sm:mt-6">
                                &mdash; Global group | Aakash N | Mumbai India
                            </footer>
                        </blockquote>
                    </CarouselItem>
                    <CarouselItem>
                        <blockquote class="px-6">
                            <p class="text-lg font-normal text-gray-800  mb-8 ">Completely drive innovative value
                                reinvent prospective whereas out-of-the-box paradigms. Interactively pursue stand-alone
                                markets after global say that they results. Professionally metrics expedite</p>
                            <footer class="mt-4 text-sm font-medium text-gray-700 sm:mt-6">
                                &mdash; Global group | Aakash N | Mumbai India
                            </footer>
                        </blockquote>
                    </CarouselItem>
                </CarouselContent>
                <CarouselPrevious />
                <CarouselNext />
            </Carousel>
        </div>
    </div>
</template>