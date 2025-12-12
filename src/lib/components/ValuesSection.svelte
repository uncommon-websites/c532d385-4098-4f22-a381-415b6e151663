<script lang="ts">
  const photos = [
    {
      title: "Embedded in Your Team",
      desc: "We work directly alongside your team—in Slack, in meetings, in the day-to-day. You get a COO without the full-time commitment.",
      img: "https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&q=80&w=400"
    },
    {
      title: "Remote-First, Globally Available",
      desc: "Our fractional model means we can support founders anywhere. Whether you're in SF, NYC, or remote, we're there when you need us.",
      img: "https://images.unsplash.com/photo-1588196749597-9ff075ee6b5b?auto=format&fit=crop&q=80&w=400"
    },
    {
      title: "Systems That Scale",
      desc: "We don't just solve today's problems—we build systems that grow with you. From seed to Series A and beyond.",
      img: "https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&q=80&w=400"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-xl mb-16">
    <h3 class="text-lg font-bold mb-2">How we work with founders.</h3>
    <p class="text-gray-500 text-sm leading-relaxed">
      We're not traditional consultants. We embed directly into your operations, working as an extension of your team. You get the strategic thinking of a COO with the hands-on execution of an operator—without the full-time cost.
    </p>
  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
    {#each photos as photo}
      <div>
        <div class="aspect-[3/4] rounded-lg overflow-hidden mb-4 bg-gray-100">
          <img src={photo.img} alt={photo.title} class="w-full h-full object-cover" />
        </div>
        <h4 class="text-xs font-bold mb-1">{photo.title}</h4>
        <p class="text-[10px] text-gray-500 leading-relaxed">{photo.desc}</p>
      </div>
    {/each}
  </div>
</section>
