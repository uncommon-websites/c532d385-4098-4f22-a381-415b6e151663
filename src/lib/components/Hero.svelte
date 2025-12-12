<script lang="ts">
  // Logos of YC-backed and startup ecosystem companies
  const logos = [
    "Y Combinator",
    "Stripe",
    "Airbnb",
    "Notion",
    "Figma"
  ];
</script>

<section class="relative min-h-screen flex flex-col justify-end pb-20 px-6 md:px-12 bg-gradient-to-b from-gray-950 via-gray-800 to-white text-[#1a1a1a]">
  <!-- Gradient overlay/background handling -->
  <div class="absolute inset-0 z-[-1] bg-[linear-gradient(180deg,oklch(0.141_0.005_285.823)_0%,oklch(0.274_0.006_286.033)_40%,oklch(0.705_0.015_286.067)_70%,#fff_100%)]"></div>

  <div class="max-w-4xl mb-32 pt-40">
    <h1 class="text-3xl md:text-5xl font-medium leading-[1.15] tracking-tight">
      Stop firefighting. Start leading. <span class="text-gray-500">Vira delivers operational clarity for overwhelmed founders through fractional COO support and embedded systems—without the full-time overhead.</span>
    </h1>
  </div>

  <div class="border-t border-gray-300 pt-8 flex flex-wrap gap-8 md:gap-16 items-center opacity-60 grayscale">
    {#each logos as logo}
      <div class="h-8 flex items-center justify-center font-bold text-xl">{logo}</div>
    {/each}
    <!-- Add more specific logo placeholders if needed -->
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
    <div class="h-8 w-20 bg-gray-400/20 rounded"></div>
  </div>
</section>
