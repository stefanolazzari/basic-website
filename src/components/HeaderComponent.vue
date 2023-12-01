<template>

  <Disclosure as="nav" class="bg-black/0" v-slot="{ open }">
    <div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
      <div class="relative flex h-16 items-center justify-between">
        <div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
          <!-- Mobile menu button-->
          <DisclosureButton class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-800 hover:bg-grey-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white">
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
                <router-link :class="[this.$route.name == item.name ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" :to="item.href">{{item.name}}</router-link>
             </div>

              <!-- <router-link :class="[this.$route.name == 'Home' ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/">Home</router-link>
              <router-link :class="[this.$route.name == 'About' ? 'bg-yellow-300 text-black' : 'text-red-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/about">About</router-link>
              <router-link :class="[this.$route.name == 'Cv' ? 'bg-yellow-300 text-black' : 'text-green-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/cv">CV</router-link>
              <router-link :class="[this.$route.name == 'Projects' ? 'bg-yellow-300 text-black' : 'text-pink-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/projects">Projects</router-link>
              <router-link :class="[this.$route.name == 'Metodo' ? 'bg-yellow-300 text-black' : 'text-orange-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/metodo">Metodo</router-link>
              <router-link :class="[this.$route.name == 'Contatti' ? 'bg-yellow-300 text-black' : 'text-blue-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/contatti">Contatti</router-link> -->
      
              <!-- <a :class="[this.$route.name == 'Home' ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/">Home</a>
              <a :class="[this.$route.name == 'About' ? 'bg-yellow-300 text-black' : 'text-red-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/about">About</a>
              <a :class="[this.$route.name == 'Cv' ? 'bg-yellow-300 text-black' : 'text-green-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/cv">CV</a>
              <a :class="[this.$route.name == 'Projects' ? 'bg-yellow-300 text-black' : 'text-pink-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/projects">Projects</a>
              <a :class="[this.$route.name == 'Metodo' ? 'bg-yellow-300 text-black' : 'text-orange-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/metodo">Metodo</a>
              <a :class="[this.$route.name == 'Contatti' ? 'bg-yellow-300 text-black' : 'text-blue-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" href="/contatti">Contatti</a> -->

   
              <!-- <a v-for="item in navigation" :key="item.name" :href="item.href" :class="[item.current ? 'bg-yellow-300 text-black' : 'text-yellow-500 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</a> -->
               <!-- <router-link v-for="item in navigation" :key="item.name" :href="item.href" :class="[item.current ? 'bg-yellow-300 text-black' : 'text-yellow-500 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" :aria-current="item.current ? 'page' : undefined">{{ item.name }}</router-link> -->

            
            </div>
          </div>
        </div>
        <!-- <div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0"> -->
          <!-- <button type="button" class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
            <span class="absolute -inset-1.5" />
            <span class="sr-only">View notifications</span>
            <BellIcon class="h-6 w-6" aria-hidden="true" />
          </button> -->

          <!-- Profile dropdown -->
          <!-- <Menu as="div" class="relative ml-3">
            <div>
              <MenuButton class="relative flex rounded-full bg-gray-800 text-sm focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
                <span class="absolute -inset-1.5" />
                <span class="sr-only">Open user menu</span>
                <img class="h-8 w-8 rounded-full" src="" alt="" />
              </MenuButton>
            </div>
            <transition enter-active-class="transition ease-out duration-100" enter-from-class="transform opacity-0 scale-95" enter-to-class="transform opacity-100 scale-100" leave-active-class="transition ease-in duration-75" leave-from-class="transform opacity-100 scale-100" leave-to-class="transform opacity-0 scale-95">
              <MenuItems class="absolute right-0 z-10 mt-2 w-48 origin-top-right rounded-md bg-white py-1 shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none">
                <MenuItem v-slot="{ active }">
                  <a href="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Your Profile</a>
                </MenuItem>
                <MenuItem v-slot="{ active }">
                  <a href="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Settings</a>
                </MenuItem>
                <MenuItem v-slot="{ active }">
                  <a href="#" :class="[active ? 'bg-gray-100' : '', 'block px-4 py-2 text-sm text-gray-700']">Sign out</a>
                </MenuItem>
              </MenuItems>
            </transition>
          </Menu> -->
        <!-- </div> -->
      </div>
    </div>

    <DisclosurePanel class="sm:hidden">
      <div class="space-y-4 px-2 pb-3 pt-2">
        <div v-for="item in navigation" :key="item.name">
          <router-link :class="[this.$route.name == item.name ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" :to="item.href">{{item.name}}</router-link>
        </div>
      </div>
    </DisclosurePanel>
    
  </Disclosure>
</template>

<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel, Menu, MenuButton, MenuItem, MenuItems } from '@headlessui/vue'
import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline'

const navigation = [
  { name: 'Home', href: '/', current: true },
  { name: 'About', href: '/about', current: false },
  { name: 'Projects', href: '/projects', current: false },
  { name: 'CV', href: '/cv', current: false },
  { name: 'Metodo', href: '/metodo', current: false },
  { name: 'Contatti', href: '/contatti', current: false },
]
</script>