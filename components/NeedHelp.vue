<script setup lang="ts">
import { Button } from '@/components/ui/button'
import { Input } from '@/components/ui/input'
import { Label } from '@/components/ui/label'
import { Textarea } from '@/components/ui/textarea'

import { Separator } from '@/components/ui/separator'
</script>
<template>
    <div class=" bg-white p-4 md:p-8 lg:p-12  ">
        <div class="xl:container">
            <div class="grid grid-cols-2 gap-4 py-4 xl:py-16  ">
                <div class="">
                    <h2 class="text-xl md:text-2xl lg:text-4xl font-bold mb-4 text-black">Unsure which plan or product
                        suits your business needs? </h2>
                    <img src="@/assets/images/need-help-avatar.png" class="w-full mx-auto max-w-md" />
                </div>
                <div>
                    <div class="w-full border rounded-lg shadow-xl">
                        <div class="flex items-center justify-center py-12">
                            <div class="mx-auto grid w-[400px] gap-6">
                                <div class="grid gap-2 text-center">
                                    <h1 class="text-3xl font-bold">
                                        Write to us
                                    </h1>
                                    <p class="text-balance text-muted-foreground">
                                        Fill out the form,
                        and our team will get back to you soon!
                                    </p>
                                </div>
                                <div class="grid gap-4">
                                    <div class="grid gap-2">
                                        <Label for="name">Name</Label>
                                        <Input id="name" type="text" placeholder="name" required />
                                    </div>
                                    <div class="grid gap-2">
                                        <Label for="email">Email</Label>
                                        <Input id="email" type="email" placeholder="m@example.com" required />
                                    </div>
                                    <div class="grid gap-2">
                                        <Label for="mobile">Mobile</Label>
                                        <Input id="mobile" type="number" placeholder="Mobile" required />
                                    </div>
                                    <div class="grid gap-2">
                                        <Label for="message">Message</Label>
                                        <Textarea placeholder="Type your message here." />
                                    </div>
                                   

                                    <Button type="submit" class="w-full bg-brand hover:bg-orange-500 p-6">
                                        Submit
                                    </Button>
                                    
                                </div>
                                <Separator class="my-4" label="OR" />
                                <Button variant="outline" class="w-full p-4">
                                        getcrm@corelto.com
                                    </Button>
                                    
                                <div class="text-center text-sm">
                                    Call us
                                    <a href="#" class="underline">
                                        +91 9812345678
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
