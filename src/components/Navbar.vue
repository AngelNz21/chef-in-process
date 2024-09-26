<template>
  <header class="bg-white shadow h-16 flex justify-between items-stretch">
    <router-link
      :to="{ name: 'home' }"
      class="inline-flex items-center px-5 h-full text-blue-400 transition-colors hover:bg-blue-400 hover:text-white font-bold"
      id="home"
    >
      Home
    </router-link>
    <div class="flex items-center gap-1">
      <router-link
        :to="{ name: 'byName' }"
        class="inline-flex items-center px-2 h-full text-blue-400 transition-colors hover:bg-blue-400 hover:text-white"
        id="search"
      >
        Search
      </router-link>
      <router-link
        :to="{ name: 'byLetter' }"
        class="inline-flex items-center px-2 h-full text-blue-400 transition-colors hover:bg-blue-400 hover:text-white"
        id="bylet"
      >
        By Letter
      </router-link>
      <router-link
        :to="{ name: 'ingredients' }"
        class="inline-flex items-center px-2 h-full text-blue-400 transition-colors hover:bg-blue-400 hover:text-white"
        id="bying"
      >
        By Ingredients
      </router-link>
    </div>
  </header>
</template>

<style>
header {
  border-radius: 0 0 20px 20px;
}
#home {
  border-radius: 0 0 0 20px;
}
#bying {
  border-radius: 0 0 20px 0;
}
</style>