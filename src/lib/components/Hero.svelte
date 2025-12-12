<script lang="ts">
  const logos = [
    "Waternet",
    "Mercedes Benz",
    "Kwik Fit",
    "HAN",
    "Hoogheemraadschap Delfland"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-white via-gray-50 to-white text-[#1a1a1a]">
  <!-- Subtle gradient background -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,#ffffff_0%,#f9fafb_50%,#ffffff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Talent creëer je niet, dat benut je. <span class="text-gray-500">Transform your career through structured talent discovery and Insights Discovery profiling. We help mid-career professionals find direction and unlock their natural potential.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60">
    <p class="text-xs uppercase tracking-wide text-gray-400 font-medium">Trusted by</p>
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-medium text-lg text-gray-600">{logo}</div>
    {/each}
  </div>
</section>
