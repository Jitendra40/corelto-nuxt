<script setup lang="ts">
import { Tabs, TabsContent, TabsList, TabsTrigger, } from '@/components/ui/tabs'
import { Separator } from '@/components/ui/separator'

import { Button } from '@/components/ui/button'
</script>
<template>
  <div class=" bg-white p-4 md:p-8 lg:p-12 mt-16 ">
    <div class="xl:container">
    <div class="text-center">
      <h2 class="text-xl md:text-2xl lg:text-4xl font-bold mb-4 text-black">Lead Protection Solution </h2>
      <p class="text-lg font-normal text-gray-800 max-w-xl text-center m-auto mb-12">Our products provide lead
        protection and drive real estate sales growth for builders and brokers. Here are our key solutions</p>
    </div>

    <Tabs default-value="builders" class="w-full ">
      <TabsList class="grid  grid-cols-2  bg-banner rounded-lg">
        <TabsTrigger value="builders" class="p-3">
          <div class="flex gap-4">
            <img src="@/assets/images/builder.svg" alt="" class="h-12 opacity-70" />
            <div class="text-left">
              <span class="bg-brand text-white rounded-sm p-1  text-xs leading-none inline-flex">Lead Protection</span>
              <span class="block text-xl">for Builders</span>
            </div>
          </div>
        </TabsTrigger>
        <TabsTrigger value="brokers" class="p-3">
          <div class="flex gap-4">
            <img src="@/assets/images/broker.svg" alt="" class="h-12 opacity-70" />
            <div class="text-left">
              <span class="bg-brand text-white rounded-sm p-1  text-xs leading-none inline-flex">Lead Protection</span>
              <span class="block text-xl">for Brokers</span>
            </div>
          </div>
        </TabsTrigger>
      </TabsList>
      <TabsContent value="builders">
        <div class="grid grid-cols-3 gap-4 py-4 xl:py-16 items-center border-b">
          <div class="">
            <img src="@/assets/images/protection160.png" alt="" class="mx-auto " />
            <span class="text-black text-xl text-center block my-4">Lead Protection</span>
          </div>
          <div class="col-span-2">
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/lead-quest.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Lead Quest</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Lead Quest Pre Sales CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  A CRM software for streamlining real estate sales while tracking marketing ROI with
                  lead management analytics & reports
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
                
              </div>
            </div>
            <Separator class="my-4" label="&" />
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/money-map.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Money Map</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Money Map Post Sales CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Streamline your inventory management from booking to possession combined with
                  powerful features and seamless automation for hassle-free post-sales processes.
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
              </div>
            </div>

          </div>

          

          
        </div>


        <div class="grid grid-cols-3 gap-4 py-4 xl:py-16 items-center border-b">
          <div >
            <img src="@/assets/images/protection180.png" alt="" class="mx-auto" />
            <span class="text-black text-xl text-center block my-4">Lead Protection</span>
          </div>
          <div class="col-span-2">
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-amber-50">
              <img src="@/assets/images/lead-quest.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Lead Quest</h3>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  A Pre Sales CRM software for streamlining real estate sales while tracking marketing ROI with
                  lead management analytics & reports
                </p>
             
                
              </div>
            </div>
            <Separator class="my-4" label="&" />
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-green-50">
              <img src="@/assets/images/money-map.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Money Map</h3>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  A Post Sales CRM Streamline your inventory management from booking to possession combined with
                  powerful features and seamless automation for hassle-free post-sales processes.
                </p>
              </div>
            </div>
            <Separator class="my-4" label="&" />
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/channel-partner.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Broker Bridge</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Broker Bridge Sourcing Team Tracking CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Seamless Real Estate Collaboration Unite Brokers, Buyers, and the Builder on a Transparent Platform. Track Performance and Status of bookings, Ensuring Customer Satisfaction Across all Channels.
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
              </div>
            </div>


          </div>

          

          
        </div>

        <div class="grid grid-cols-3 gap-4 py-4 xl:py-16 items-center border-b">
          <div >
            <img src="@/assets/images/protection360.png" alt="" class="mx-auto" />
            <span class="text-black text-xl text-center block my-4">Lead Protection</span>
          </div>
          <div class="col-span-2">
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-amber-50">
              <img src="@/assets/images/lead-quest.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Lead Quest</h3>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  A Pre Sales CRM software for streamlining real estate sales while tracking marketing ROI with
                  lead management analytics & reports
                </p>
             
                
              </div>
            </div>
            <Separator class="my-4" label="&" />
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-green-50">
              <img src="@/assets/images/money-map.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Money Map</h3>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  A Post Sales CRM Streamline your inventory management from booking to possession combined with
                  powerful features and seamless automation for hassle-free post-sales processes.
                </p>
              </div>
            </div>
            <Separator class="my-4" label="&" />
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-orange-50">
              <img src="@/assets/images/channel-partner.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Broker Bridge</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Broker Bridge Sourcing Team Tracking CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Seamless Real Estate Collaboration Unite Brokers, Buyers, and the Builder on a Transparent Platform. Track Performance and Status of bookings, Ensuring Customer Satisfaction Across all Channels.
                </p>
            
              </div>
            </div>
            <Separator class="my-4" label="&" />

            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/virtual-tour.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Virtual Visit</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Virtual Site Visit & Booking Tool CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Empower customers to book dream homes online via our cutting-edge online booking platform, offering virtual site visits and complete transparency on the project.
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
              </div>
            </div>


          </div>

          

          
        </div>


      </TabsContent>
      <TabsContent value="brokers">
        <div class="grid grid-cols-3 gap-4 py-4 xl:py-16 items-center border-b">
          <div >
            <img src="@/assets/images/protection180.png" alt="" class="mx-auto" />
            <span class="text-black text-xl text-center block my-4">Lead Protection</span>
          </div>
          <div class="col-span-2">
            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/lead-hub.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Lead Hub</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Channel partner CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Streamline your broking business flawlessly with our next-gen CRM software designed for channel partners, featuring comprehensive workflow management and automation.
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
                
              </div>
            </div>
          </div>

          

          
        </div>

        <div class="grid grid-cols-3 gap-4 py-4 xl:py-16 items-center border-b">
          <div >
            <img src="@/assets/images/protection360.png" alt="" class="mx-auto" />
            <span class="text-black text-xl text-center block my-4">Lead Protection</span>
          </div>
          <div class="col-span-2">

            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6 bg-orange-50">
              <img src="@/assets/images/lead-hub.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Lead Hub</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Channel partner CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Streamline your broking business flawlessly with our next-gen CRM software designed for channel partners, featuring comprehensive workflow management and automation.
                </p>
            
              </div>
            </div>
            <Separator class="my-4" label="&" />

            <div class="flex gap-4  p-4 rounded-lg lg:gap-6 mb-2 lg:mb-6">
              <img src="@/assets/images/channel-collect.svg" alt="" class="h-14 opacity-70" />
              <div class="flex flex-col gap-2 ">
                <h3 class="text-xl font-medium leading-none">Channel Collect</h3>
                <h4 class="text-md font-medium text-gray-800">Discover the prower of Channel collect post sales CRM</h4>
                <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                  Master your Channel Partner cash-flows: Track brokerage inflow status,incentive payout and conquer your AOP effortlessly!
                </p>
                <div class="grid grid-cols-2 gap-4 mt-4">
                  <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/centralized-lead.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Centralized Lead Management</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Quest centralizes lead management by capturing leads from multiple digital channels,
                    including landing pages, social media, and live chat.
                </p>
                </div>
                <div class="flex gap-2 flex-col items-start">
                  <img src="@/assets/images/lead-capture.svg" alt="" class="h-10 opacity-80" />
                  <h4 class="text-md font-medium text-gray-800">Real-Time Lead Capture</h4>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    With Quest, leads are instantly captured in real-time from digital campaigns, including Facebook, Magicbricks, 99acres, and websites. 
                </p>
                </div>
                </div>
                
                <div class="flex gap-4 mt-4">
                  <Button variant="outline">Discover more</Button>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
                
              </div>
            </div>
           

          </div>

          

          
        </div>
      </TabsContent>

    </Tabs>
  </div>

  </div>
</template>