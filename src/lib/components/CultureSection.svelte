<script lang="ts">
  const cards = [
    {
      title: "We Don't Create Talent...",
      subtitle: "We Help You Utilize It.",
      image: "https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?auto=format&fit=crop&q=80&w=800"
    },
    {
      title: "We Don't Follow Templates...",
      subtitle: "We Discover Your Unique Path.",
      image: "https://images.unsplash.com/photo-1531482615713-2afd69097998?auto=format&fit=crop&q=80&w=800"
    },
    {
      title: "We Don't Offer Quick Fixes...",
      subtitle: "We Build Lasting Transformation.",
      image: "https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&q=80&w=800"
    }
  ];
</script>

<section class="py-24 px-6 md:px-12 bg-white">
  <div class="max-w-2xl mb-16">
    <p class="text-xl md:text-2xl leading-relaxed text-gray-800">
      When people use their natural talents, they experience more energy, satisfaction, and pleasure in both work and personal life. Our approach combines 25 years of human development expertise with proven Insights Discovery methodology.
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
           <span>→</span>
        </div>
      </div>
    {/each}
  </div>
</section>
