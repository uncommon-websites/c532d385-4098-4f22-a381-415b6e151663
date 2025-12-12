<script lang="ts">
  const founders = [
    {
      name: "Agustin Campos",
      title: "Strategy Director",
      image: "https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&q=80&w=200"
    },
    {
      name: "Mateo Costa",
      title: "CEO & Co-Founder",
      image: "https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?auto=format&fit=crop&q=80&w=200"
    }
  ];
</script>

<section class="px-6 md:px-12 py-24 bg-white">
  <div class="rounded-2xl overflow-hidden relative bg-gradient-to-br from-gray-950 to-primary-900 text-white p-8 md:p-16 min-h-[600px] flex flex-col justify-between">
    <div class="max-w-2xl">
      <h2 class="text-3xl md:text-5xl font-bold mb-6 leading-tight">Ready to build your dream team?</h2>
      <p class="text-lg md:text-xl text-gray-300 mb-8">Stop losing sleep over hiring. Let's create a system that brings you top talent consistently.</p>
      
      <div class="flex flex-col sm:flex-row gap-4 mb-12">
        <div class="bg-white/10 backdrop-blur-sm rounded-lg p-4 flex-1">
          <div class="text-2xl font-bold mb-1">No retainers</div>
          <div class="text-sm text-gray-300">Pay only for successful hires</div>
        </div>
        <div class="bg-white/10 backdrop-blur-sm rounded-lg p-4 flex-1">
          <div class="text-2xl font-bold mb-1">90-day guarantee</div>
          <div class="text-sm text-gray-300">We stand behind every placement</div>
        </div>
      </div>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 max-w-4xl">
      {#each founders as founder}
        <div class="bg-white text-black rounded-xl p-6 flex items-center gap-6">
          <div class="w-20 h-20 rounded-lg overflow-hidden bg-gray-200 shrink-0">
            <img src={founder.image} alt={founder.name} class="w-full h-full object-cover" />
          </div>
          <div class="flex-1">
            <h3 class="font-bold text-lg mb-1">{founder.name}</h3>
            <p class="text-xs text-gray-500 mb-4">{founder.title}</p>
            <button class="bg-black text-white px-6 py-2 rounded-full text-xs font-bold uppercase tracking-wide hover:bg-gray-800 transition-colors">
              Book a call
            </button>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
