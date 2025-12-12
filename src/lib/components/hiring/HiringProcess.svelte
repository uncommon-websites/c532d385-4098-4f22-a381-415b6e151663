<script lang="ts">
  const steps = [
    {
      number: "01",
      title: "Discovery & strategy",
      description: "We start by understanding your needs, culture, and growth plans. Together, we define the ideal candidate profile and build a targeted sourcing strategy.",
      duration: "Week 1"
    },
    {
      number: "02",
      title: "Sourcing & screening",
      description: "Our team activates our network and sourcing channels. We handle initial screenings, technical assessments, and culture fit evaluations.",
      duration: "Weeks 2-3"
    },
    {
      number: "03",
      title: "Candidate presentation",
      description: "You receive a curated shortlist of pre-vetted candidates with detailed profiles. We coordinate interviews and gather feedback at every stage.",
      duration: "Week 3-4"
    },
    {
      number: "04",
      title: "Offer & onboarding",
      description: "We manage offer negotiations and create a seamless onboarding experience. Our support continues through the first 90 days to ensure success.",
      duration: "Week 4+"
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-gray-50">
  <div class="max-w-6xl mx-auto">
    <div class="mb-16 text-center">
      <h2 class="text-3xl md:text-4xl font-bold mb-4">How it works</h2>
      <p class="text-lg text-gray-600 max-w-2xl mx-auto">A proven process that delivers quality hires in weeks, not months. Transparent, efficient, and designed for startup speed.</p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      {#each steps as step}
        <div class="bg-white rounded-xl p-8 border border-gray-200">
          <div class="flex items-start justify-between mb-6">
            <div class="text-5xl font-bold text-gray-200">{step.number}</div>
            <div class="text-xs uppercase tracking-wider text-gray-500 bg-gray-100 px-3 py-1 rounded-full">{step.duration}</div>
          </div>
          <h3 class="text-2xl font-bold mb-4">{step.title}</h3>
          <p class="text-gray-600 leading-relaxed">{step.description}</p>
        </div>
      {/each}
    </div>

    <div class="mt-16 bg-white rounded-xl p-8 md:p-12 border border-gray-200">
      <div class="flex flex-col md:flex-row items-start md:items-center justify-between gap-6">
        <div class="flex-1">
          <h3 class="text-2xl font-bold mb-2">Not sure where to start?</h3>
          <p class="text-gray-600">Book a free consultation to discuss your hiring needs and see if we're a good fit.</p>
        </div>
        <button class="bg-black text-white px-8 py-3 rounded-full text-sm font-bold uppercase tracking-wide hover:bg-gray-800 transition-colors whitespace-nowrap">
          Schedule a call
        </button>
      </div>
    </div>
  </div>
</section>
