<template>
  <nav
    class="top-0 fixed z-50 w-full flex flex-wrap items-center justify-between px-2 py-3 navbar-expand-lg bg-white shadow">
    <div class="container px-4 mx-auto flex flex-wrap items-center justify-between">
      <div class="w-full relative flex justify-between lg:w-auto lg:static lg:block lg:justify-start">
        <router-link to="/">
          <a class="text-blueGray-700 text-sm font-bold leading-relaxed inline-block mr-4 py-2 whitespace-nowrap uppercase"
            href="#pablo">
            Book donation system
          </a>
        </router-link>
      </div>
      <div class="lg:flex flex-grow items-center" :class="[navbarOpen ? 'block' : 'hidden']" id="example-navbar-warning">
        <ul class="flex flex-col lg:flex-row list-none lg:ml-auto">
          <li class="flex items-center">
            <button
              class="bg-emerald-500 text-white active:bg-emerald-600 text-xs font-bold uppercase px-4 py-2 rounded shadow hover:shadow-lg outline-none focus:outline-none lg:mr-1 lg:mb-0 ml-3 mb-3 ease-linear transition-all duration-150"
              type="button">
              <i class="fas fa-sign-in-alt"></i> Login
            </button>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>

</script>
