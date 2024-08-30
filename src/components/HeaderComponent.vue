<template>

  <Disclosure as="nav" class="pt-10" v-slot="{ open }">
    <div class="bg-black/10 mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-16 items-center justify-between">
        <div class=" absolute inset-y-0 left-0 flex items-center sm:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton class="relative inline-flex items-center justify-center rounded-md p-2 text-black hover:bg-yellow-300 hover:text-black focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white">
            <span class="absolute -inset-0.5" />
            <span class="sr-only">Open main menu</span>
            <Bars3Icon v-if="!open" class="block h-6 w-6" aria-hidden="true" />
            <XMarkIcon v-else class="block h-6 w-6" aria-hidden="true" />
          </DisclosureButton>
        </div>

        
        <div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
          <div class="flex flex-shrink-0 items-center">
          </div>
          <div class="hidden sm:ml-6 sm:block">
            <div class="flex space-x-4">

              <div v-for="item in navigation" :key="item.name">
                <!-- <router-link :class="[this.$route.name == item.name ? 'bg-yellow-300 text-black' : 'text-yellow-300 bg-black/70 hover:bg-gray-700 hover:text-black', 'rounded-md px-3 py-2 text-sm font-medium']" :to="item.href">{{item.name}}</router-link> -->
                <router-link class="text-yellow-300 bg-black/70 hover:bg-pink-600 hover:text-black rounded-md px-3 py-2 text-sm font-medium" active-class="menu-hl"  :to="item.href">{{item.name}}</router-link>
              </div>
            
            </div>
          </div>
        </div>
      </div>
    </div>

    <DisclosurePanel class="sm:hidden">
      <div class="space-y-4 px-2 pb-3 pt-2">
        <div v-for="item in navigation" :key="item.name">
          <div active-class="menu-hl" class="bg-black/70 text-yellow-300 rounded-md px-3 py-2 hover:bg-yellow-300 hover:text-pink-500 text-sm font-medium" >
          <!-- <router-link :class="[this.$route.name == item.name ? 'bg-yellow-300 text-black' : 'text-yellow-300 bg-black/70 hover:bg-gray-700 hover:text-black', 'rounded-md px-3 py-2 text-sm font-medium']" :to="item.href">{{item.name}}</router-link> -->
          <router-link :to="item.href">{{item.name}}</router-link>
         </div>
        </div>
      </div>
    </DisclosurePanel>
    <hr>
    
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'

const navigation = [
  { name: 'Home', href: '/', current: true },
  { name: 'Competenze', href: '/competenze', current: false },
  { name: 'Projects', href: '/projects', current: false },
  { name: 'Contatti', href: '/contatti', current: false },
  { name: 'Corsi', href: '/corsi', current: false },
]
</script>

