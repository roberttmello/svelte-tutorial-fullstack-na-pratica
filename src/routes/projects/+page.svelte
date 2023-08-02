<script>
  export let data;
</script>

<section class="bg-white dark:bg-gray-900">
  <div class="container px-6 mx-auto">
    <div class="flex py-4 mt-4 overflow-x-auto overflow-y-hidden md:justify-center dark:border-gray-700">
      <button class="h-12 px-8 py-2 -mb-px text-sm text-center text-blue-600 bg-transparent border-b-2 border-blue-500 sm:text-base dark:border-blue-400 dark:text-blue-300 whitespace-nowrap focus:outline-none">
                Animation
            </button>

            <button
                class="h-12 px-8 py-2 -mb-px text-sm text-center text-gray-700 bg-transparent border-b-2 border-gray-200 sm:text-base dark:text-white whitespace-nowrap cursor-base focus:outline-none dark:border-gray-700 dark:hover:border-gray-400 hover:border-gray-400">
                Web design
            </button>

            <button
                class="h-12 px-8 py-2 -mb-px text-sm text-center text-gray-700 bg-transparent border-b-2 border-gray-200 sm:text-base dark:text-white whitespace-nowrap cursor-base focus:outline-none dark:border-gray-700 dark:hover:border-gray-400 hover:border-gray-400">
                App design
            </button>

            <button
                class="h-12 px-8 py-2 -mb-px text-sm text-center text-gray-700 bg-transparent border-b-2 border-gray-200 sm:text-base dark:text-white whitespace-nowrap cursor-base focus:outline-none dark:border-gray-700 dark:hover:border-gray-400 hover:border-gray-400">
                Branding
            </button>
        </div>

        <section class="mt-8 space-y-8 lg:mt-12">

            {#each data.items  as {title, category, imageUrl} }
              <section class="lg:flex lg:items-center">
                  <div class="lg:w-1/2 ">
                      <p class="text-lg tracking-wider text-blue-500 uppercase dark:text-blue-400 ">{category}</p>
                      <h2 class="mt-2 text-2xl font-semibold text-gray-800 capitalize dark:text-white">{title}</h2>
                  </div>

                  <div class="mt-4 lg:w-1/2 lg:mt-0">
                    <img class="object-cover w-full h-64 rounded-lg md:h-96"
                      src={imageUrl} alt="Porfolio">
                  </div>
              </section>
            {/each}

        </section>
  </div>
</section>
