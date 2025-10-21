<script setup lang="ts">
defineProps({
  title: { type: String, required: true },
  description: { type: String, required: true },
  imgUrl: { type: String, required: true },
  icon: { type: String },
  category: { type: String },
});
</script>
<template>
  <div class="flex justify-center items-center p-2 h-full">
    <div
      class="position-relative w-full h-full max-w-sm sm:max-w-md md:max-w-xl lg:max-w-2xl mx-auto bg-white/5 backdrop-blur-xl border border-white/10 rounded-3xl p-6 shadow-2xl shadow-indigo-900/50 hover:shadow-cyan-500/50 transform transition-all duration-500 card-glow"
    >
      <!-- Image Section with inner rounded corners -->
      <div class="relative w-full h-52 sm:h-64 mb-6">
        <img
          class="absolute inset-0 w-full h-full object-cover rounded-2xl border border-white/5"
          :src="imgUrl"
        />
        <!-- Optional: Overlay for subtle effects -->
        <div
          class="absolute inset-0 rounded-2xl bg-gradient-to-t from-transparent via-transparent to-black/20"
        ></div>
      </div>

      <!-- Content Area -->
      <div class="text-white">
        <h5
          id="project-title"
          class="text-3xl sm:text-4xl font-bold leading-tight mb-2 text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-purple-400"
        >
          {{ title }}
        </h5>
        <p class="text-indigo-300 text-sm sm:text-base font-medium mb-4">
          {{ category || "Web Application" }}
        </p>
        <p
          id="project-description"
          class="dark:text-gray-200 text-sm sm:text-base leading-relaxed mb-6 text-black/100"
        >
          {{ description }}
        </p>
      </div>

      <!-- Technology Stack -->
      <div
        class="mt-8 pt-6 border-t dark:border-white/10 flex flex-wrap items-center gap-3"
      >
        <span
          class="text-gray-300 flex items-center space-x-1 text-sm dark:bg-white/5 px-3 py-1 rounded-full border dark:border-white/10"
        >
          <svg
            class="h-4 w-4 text-sky-400"
            fill="currentColor"
            viewBox="0 0 20 20"
          >
            <!-- Generic Icon for tech stack -->
            <path
              fill-rule="evenodd"
              d="M10 18a8 8 0 100-16 8 8 0 000 16zM8 11a1 1 0 112 0 1 1 0 01-2 0zm4 0a1 1 0 112 0 1 1 0 01-2 0zM10 7a1 1 0 100 2 1 1 0 000-2z"
              clip-rule="evenodd"
            />
          </svg>
          <span class="text-black/100 dark:text-gray-200">React</span>
        </span>
      </div>

    </div>
  </div>
</template>
