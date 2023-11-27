<template>
              <router-link :class="[this.$route.name == 'Home' ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/">Home</router-link>
              <router-link :class="[this.$route.name == 'About' ? 'bg-yellow-300 text-black' : 'text-red-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/about">About</router-link>
              <router-link :class="[this.$route.name == 'Cv' ? 'bg-yellow-300 text-black' : 'text-green-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/cv">CV</router-link>
              <router-link :class="[this.$route.name == 'Projects' ? 'bg-yellow-300 text-black' : 'text-pink-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/projects">Projects</router-link>
              <router-link :class="[this.$route.name == 'Metodo' ? 'bg-yellow-300 text-black' : 'text-orange-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/metodo">Metodo</router-link>
              <router-link :class="[this.$route.name == 'Contatti' ? 'bg-yellow-300 text-black' : 'text-blue-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/contatti">Contatti</router-link>
      
      
            <Disclosure>
                <DisclosureButton>
                Is team pricing available?
                </DisclosureButton>
                <DisclosurePanel >
                    <router-link :class="[this.$route.name == 'Home' ? 'bg-yellow-300 text-black' : 'text-yellow-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/">Home</router-link>
              <router-link :class="[this.$route.name == 'About' ? 'bg-yellow-300 text-black' : 'text-red-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/about">About</router-link>
              <router-link :class="[this.$route.name == 'Cv' ? 'bg-yellow-300 text-black' : 'text-green-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/cv">CV</router-link>
              <router-link :class="[this.$route.name == 'Projects' ? 'bg-yellow-300 text-black' : 'text-pink-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/projects">Projects</router-link>
              <router-link :class="[this.$route.name == 'Metodo' ? 'bg-yellow-300 text-black' : 'text-orange-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/metodo">Metodo</router-link>
              <router-link :class="[this.$route.name == 'Contatti' ? 'bg-yellow-300 text-black' : 'text-blue-500 bg-black/50 hover:bg-gray-700 hover:text-white', 'rounded-md px-3 py-2 text-sm font-medium']" to="/contatti">Contatti</router-link>
                </DisclosurePanel>
            </Disclosure>
</template>

<script setup>
import { DisclosureButton, Disclosure, DisclosurePanel } from '@headlessui/vue';
</script>