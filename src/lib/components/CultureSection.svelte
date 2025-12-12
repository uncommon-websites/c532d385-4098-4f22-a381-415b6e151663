<script lang="ts">
  const cards = [
    {
      title: "We're Not Consultants...",
      subtitle: "We're Your Embedded COO.",
      image: "https://images.unsplash.com/photo-1556761175-b413da4baf72?auto=format&fit=crop&q=80&w=800"
    },
    {
      title: "We Don't Just Advise...",
      subtitle: "We Execute Alongside You.",
      image: "https://images.unsplash.com/photo-1600880292203-757bb62b4baf?auto=format&fit=crop&q=80&w=800"
    },
    {
      title: "We Don't Deliver Decks...",
      subtitle: "We Build Systems That Work.",
      image: "https://images.unsplash.com/photo-1553877522-43269d4ea984?auto=format&fit=crop&q=80&w=800"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      We're not here to hand you a strategy deck and disappear. We embed directly into your operations, working side-by-side with you to build systems that actually stick.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each cards as card}
      <div class="group">
        <div class="aspect-[4/3] overflow-hidden rounded-lg mb-4 bg-gray-100">
          <img src={card.image} alt={card.title} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
        </div>
        <h3 class="text-sm text-gray-500 mb-1">{card.title}</h3>
        <p class="text-sm font-bold">{card.subtitle}</p>
        
        <div class="flex justify-between mt-4 text-xs text-gray-400">
           <span>01</span>
           <span>-></span>
        </div>
      </div>
    {/each}
  </div>
</section>
