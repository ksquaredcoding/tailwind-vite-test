<template>
  <nav class="bg-slate-700 shadow-lg">
    <div class="flex flex-col justify-between items-center">
      <div class="my-6">
        <a href="" class="flex items-center">
          <img src="../assets/k-blue-logo.jpg" alt="K Logo" title="Home Page"
            class="object-contain w-28 h-auto rounded-full hover:border-sky-200 hover:border-2 hover:border-solid hover:shadow-lg p-3">
        </a>
      </div>
      <div class="flex flex-col px-2">
        <router-link :to="{ name: 'About' }"
          class="text-lg shrink font-bold text-emerald-50  uppercase tracking-wide hover:border-sky-200 hover:border-b-2 hover:border-solid hover:rounded hover:bg-sky-50 hover:bg-opacity-25 hover:text-sky-400 hover:shadow-lg text-shadow p-1"
          title="About Page">About</router-link>
        <router-link :to="{ name: 'Portfolio' }"
          class="text-lg shrink font-bold text-emerald-50  uppercase tracking-wide hover:border-sky-200 hover:border-b-2 hover:border-solid hover:rounded hover:bg-sky-50 hover:bg-opacity-25 hover:text-sky-400 hover:shadow-lg text-shadow p-1"
          title="Portfolio Page">Portfolio</router-link>
        <button type="button" data-modal-toggle="testModal">Modal</button>
      </div>
    </div>
  </nav>
</template>


<script>
export default {
  setup() {
    return {}
  }
}
</script>


<style lang="css" scoped>

</style>