<template>
    <div>
      <div class="sm:pl-2 sm:pr-2   lg:pl-60 lg:pr-60">
      <h1 class="p-5">{{this.$route.name}}</h1>
        <div class="grid gap-2 sm:grid-cols-1 lg:grid-cols-1">
         <div class="p-6 bg-black/70 text-yellow-300 text-center items-center rounded-md">
            <p><slot /></p>
         </div> 
      </div>
     </div>
    </div>
  </template>
  
  <script>
  
  </script>