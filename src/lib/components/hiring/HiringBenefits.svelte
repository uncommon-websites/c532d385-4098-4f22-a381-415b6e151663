<script lang="ts">
  const benefits = [
    {
      title: "Precision matching",
      description: "We don't just fill seats. Our embedded systems identify candidates who align with your culture, mission, and growth trajectory."
    },
    {
      title: "Speed without compromise",
      description: "Reduce time-to-hire by 60% with our proven process. Get qualified candidates in your pipeline within days, not months."
    },
    {
      title: "Full-cycle support",
      description: "From job description to offer acceptance, we handle every step. You focus on building; we handle the hiring operations."
    },
    {
      title: "Scalable systems",
      description: "Build hiring infrastructure that grows with you. Our embedded approach means you're not dependent on external recruiters forever."
    },
    {
      title: "Quality guaranteed",
      description: "Every candidate is thoroughly vetted. Our rigorous screening process ensures you only meet with top-tier talent."
    },
    {
      title: "Fractional flexibility",
      description: "Pay for what you need, when you need it. No retainers, no long-term contracts. Just results-driven hiring support."
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="max-w-6xl mx-auto">
    <div class="mb-16">
      <h2 class="text-3xl md:text-4xl font-bold mb-4">Why founders choose Vira for hiring</h2>
      <p class="text-lg text-gray-600 max-w-2xl">Traditional recruiting is broken. We've built a better way—one that respects your time, budget, and company culture.</p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
      {#each benefits as benefit}
        <div class="border border-gray-200 rounded-xl p-8 hover:border-gray-400 transition-colors">
          <h3 class="text-xl font-bold mb-3">{benefit.title}</h3>
          <p class="text-gray-600 leading-relaxed">{benefit.description}</p>
        </div>
      {/each}
    </div>
  </div>
</section>
