<script lang="ts">
  const stats = [
    { value: "23 days", label: "Average time to hire" },
    { value: "40%", label: "Reduction in hiring costs" },
    { value: "95%", label: "First-year retention rate" }
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-gray-950 via-gray-800 to-white text-[#1a1a1a]">
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,oklch(0.141_0.005_285.823)_0%,oklch(0.274_0.006_286.033)_40%,oklch(0.705_0.015_286.067)_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <div class="text-xs uppercase tracking-wider text-gray-400 mb-4">Hiring Services</div>
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight mb-8">
      Stop wasting months on bad hires. <span class="text-gray-500">Build your dream team faster with embedded hiring systems that actually work—from sourcing to onboarding.</span>
    </h1>
    <div class="flex flex-wrap gap-4">
      <button class="bg-black text-white px-8 py-3 rounded-full text-sm font-bold uppercase tracking-wide hover:bg-gray-800 transition-colors">
        Start hiring smarter
      </button>
      <button class="border-2 border-gray-300 text-black px-8 py-3 rounded-full text-sm font-bold uppercase tracking-wide hover:border-gray-400 transition-colors">
        See how it works
      </button>
    </div>
  </div>

  <div class="border-t border-gray-300 pt-8 grid grid-cols-1 md:grid-cols-3 gap-8">
    {#each stats as stat}
      <div>
        <div class="text-3xl md:text-4xl font-bold mb-2">{stat.value}</div>
        <div class="text-sm text-gray-600">{stat.label}</div>
      </div>
    {/each}
  </div>
</section>
