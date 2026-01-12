<script>
  let heroImage = '/generated/image-modern-warehouse-interior-with-organized-1767814296376-0.webp';
</script>

<section class="pt-20 pb-16 text-center max-w-[1200px] mx-auto px-6">
  <h1 class="text-6xl font-bold tracking-tight text-gray-900 mb-6 leading-[1.1]">
    Smarter Inventory Decisions.<br>Built for Modern Retail.
  </h1>
  <p class="text-lg text-gray-600 mb-8 max-w-2xl mx-auto leading-relaxed">
    Mercator Intelligence delivers AI-driven inventory decisioning that works within your real retail workflows—no more fragmented legacy tools.
  </p>
  <button class="bg-gray-900 text-white px-6 py-3 rounded-lg hover:bg-gray-800 transition-colors font-semibold text-sm mb-20 cursor-pointer">
    Request Demo
  </button>

  <!-- Hero Image -->
  {#if heroImage}
    <div class="relative w-full aspect-[2/1] bg-gray-50 rounded-xl overflow-hidden border border-gray-100">
      <img src={heroImage} alt="Retail inventory management" class="w-full h-full object-cover" />
      <div class="absolute inset-0 bg-gradient-to-t from-white via-transparent to-transparent pointer-events-none"></div>
    </div>
  {:else}
    <div class="relative w-full aspect-[2/1] bg-gray-50 rounded-xl overflow-hidden flex items-center justify-center border border-gray-100">
      <!-- Abstract representation of inventory flow -->
      <div class="relative w-full h-full flex items-center justify-center">
        <div class="grid grid-cols-5 gap-4 p-8">
          <!-- Warehouse boxes -->
          <div class="w-24 h-24 bg-gray-200 rounded-lg shadow-md border border-gray-300 flex items-center justify-center">
            <div class="text-3xl">📦</div>
          </div>
          <div class="w-24 h-24 bg-gray-300 rounded-lg shadow-md border border-gray-400 flex items-center justify-center">
            <div class="text-3xl">📦</div>
          </div>
          <div class="w-24 h-24 bg-primary-400 rounded-lg shadow-lg border border-primary-500 flex items-center justify-center animate-pulse">
            <div class="text-3xl">🤖</div>
          </div>
          <div class="w-24 h-24 bg-gray-300 rounded-lg shadow-md border border-gray-400 flex items-center justify-center">
            <div class="text-3xl">📦</div>
          </div>
          <div class="w-24 h-24 bg-gray-200 rounded-lg shadow-md border border-gray-300 flex items-center justify-center">
            <div class="text-3xl">📦</div>
          </div>
        </div>
      </div>
      <div class="absolute inset-0 bg-gradient-to-t from-white via-transparent to-transparent pointer-events-none"></div>
    </div>
  {/if}

  <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mt-20 text-left">
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">10102</div>
      <h3 class="text-xl font-bold text-gray-900 mb-2">AI-Driven Decisioning</h3>
      <p class="text-sm text-gray-500 leading-relaxed">
        Intelligent inventory recommendations powered by AI that understands your business context, demand patterns, and supply chain constraints.
      </p>
    </div>
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">02</div>
      <h3 class="text-xl font-bold text-gray-900 mb-2">Workflow-Native test</h3>
      <p class="text-sm text-red-500 leading-relaxed">
        Built around real retail workflows, not forcing you to adapt to rigid legacy systems. Works the way your team actually operates.
      </p>
    </div>
    <div>
      <div class="text-xs font-semibold text-gray-400 mb-2">03</div>
      <h3 class="text-xl font-bold text-green-600 mb-2">Modern Platform</h3>
      <p class="text-sm text-gray-500 leading-relaxed">
        Replace fragmented spreadsheets and outdated tools with a unified, AI-native execution layer for your entire supply chain.
      </p>
    </div>
  </div>
</section>
