<script setup lang="ts">
import { Menu } from "lucide-vue-next";
import {
  NavigationMenu,
  NavigationMenuContent,
  NavigationMenuItem,
  NavigationMenuLink,
  NavigationMenuList,
  NavigationMenuTrigger,
  navigationMenuTriggerStyle,
} from '@/components/ui/navigation-menu'

import { Sheet, SheetContent, SheetTrigger } from '@/components/ui/sheet'

const isScrolled = ref(false);

const handleScroll = () => {
  isScrolled.value = window.scrollY > 200;
};

onMounted(() => {
  window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
  window.removeEventListener('scroll', handleScroll);
});
</script>

<template>
    <header class="sticky top-0 flex h-16 items-center gap-4 border-b px-4 md:px-6 bg-transparent z-1" :class="{ 'bg-white': isScrolled }" @scroll="handleScroll">
        <nav class="hidden flex-col gap-6 text-lg font-medium md:flex md:flex-row md:items-center md:gap-5 md:text-sm lg:gap-6 w-full ">
            <div class="w-1/3">
            <a href="/" class="flex items-center gap-2 text-lg font-semibold md:text-base ">
                <img src="@/assets/images/logo.png" alt="Corelto" class="h-12" />
                <span class="sr-only">Corelto</span>
            </a>
        </div>
            <div class="flex items-center gap-6 w-1/3 justify-center">
                <NavigationMenu>
    <NavigationMenuList>
        <NavigationMenuItem >
        <NavigationMenuLink href="/" :class="navigationMenuTriggerStyle()" class="bg-transparent hover:bg-white">
            Why Corelto?
        </NavigationMenuLink>
      </NavigationMenuItem>
      <NavigationMenuItem >
        
        <NavigationMenuTrigger class="bg-transparent hover:bg-white">Products</NavigationMenuTrigger>
        <NavigationMenuContent>
          <div class="grid gap-3 p-6 md:w-[700px] lg:w-[1200px] lg:grid-cols-3">
          
            <div class="border-e p-2">
                <h2 class="mb-3 text-gray-500">Lead Protection for Builders</h2>
                <div>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Lead Quest</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                   Sales, Pre-Sales, Market Tracking CRM
                  </p>
                  </div>
                </a>
              </NavigationMenuLink>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center  select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/money-map.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Money Map</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                   Post-Sales CRM, Customer & Broker Access App 
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  
                  <div class="text-sm font-medium leading-none">Broker Bridge</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                   Channel Partner Access, Sourcing Team   
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Virtual Visit</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                   Online Site-visit, online Booking tool   
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Discover</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                   Property management platform  
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
            </div>            
            </div>
            <div class="p-2">
                <h2>Lead Protection for Brokers</h2>
                <div>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Lead Hub</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Channel partner CRM
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
              <NavigationMenuLink as-child>
                <a
                  href="/"
                  class="flex gap-4 items-center select-none space-y-1 rounded-md p-3 leading-none no-underline outline-none transition-colors hover:bg-accent hover:text-accent-foreground focus:bg-accent focus:text-accent-foreground"
                >
                <img src="@/assets/images/lead-quest.svg" alt="" class="h-12 opacity-70" />
                <div class="flex flex-col gap-2">
                  <div class="text-sm font-medium leading-none">Channel Collect</div>
                  <p class="line-clamp-2 text-sm leading-snug text-muted-foreground">
                    Channel partner Post-Sales CRM
                  </p>
                </div>
                </a>
              </NavigationMenuLink>
            </div>            
            </div>
          
            <div class="">
              <NavigationMenuLink as-child>
                <div
                  class="flex h-full w-full select-none flex-col justify-end rounded-md bg-brand-light p-6 no-underline outline-none focus:shadow-md"
                >
                
                  <img src="https://www.radix-vue.com/logo.svg" class="h-6 w-6">
                  <div class="mb-2 mt-4 text-xl font-medium">
                    Customised  Solution
                  </div>
                  <p class="text-xs leading-tight text-gray-800 mb-4">
                    In the dynamic real estate industry, a one-size-fits-all approach doesn't work. Our Customised Product Solutions are designed to meet your specific business needs, helping you streamline operations, enhance client experience, and maximize profitability.
                  </p>
                  <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>
                </div>
              </NavigationMenuLink>
            </div>
          </div>
        </NavigationMenuContent>
      </NavigationMenuItem>
 
      <NavigationMenuItem>
        <NavigationMenuLink href="/" :class="navigationMenuTriggerStyle()" class="bg-transparent hover:bg-white">
            Testimonials
        </NavigationMenuLink>
      </NavigationMenuItem>
    </NavigationMenuList>
  </NavigationMenu>
            </div>
            <div class="flex gap-4 w-1/3 justify-end">
                <div class="flex gap-2 items-center">
                    <img src="@/assets/images/call-icon.svg" alt="Corelto" class="h-8" />
                    <div class="flex flex-col">
                        <span class="text-xs text-gray-500">Call Us</span>
                        <span>+91 9812345678</span>
                    </div>
                </div>
                <Button class="bg-brand hover:bg-orange-500">Book a demo</Button>

            </div>
        </nav>
        <Sheet>
            <SheetTrigger as-child>
                <Button variant="outline" size="icon" class="shrink-0 md:hidden">
                    <Menu class="h-5 w-5" />
                    <span class="sr-only">Toggle navigation menu</span>
                </Button>
            </SheetTrigger>
            <SheetContent side="left">
                <nav class="grid gap-6 text-lg font-medium">
                    <a href="#" class="flex items-center gap-2 text-lg font-semibold">
                        <Package2 class="h-6 w-6" />
                        <span class="sr-only">Acme Inc</span>
                    </a>
                    <a href="#" class="text-foreground transition-colors hover:text-foreground">
                        Why Corelto?
                    </a>
                    <a href="#" class="text-muted-foreground transition-colors hover:text-foreground">
                        Products
                    </a>
                    <a href="#" class="text-muted-foreground transition-colors hover:text-foreground">
                        Testimonials
                    </a>
                </nav>
            </SheetContent>
        </Sheet>
    </header>
</template>
