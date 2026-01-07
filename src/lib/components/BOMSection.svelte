<script>
</script>

<section class="bg-[#0B0F19] text-white py-24">
  <div class="max-w-[1200px] mx-auto px-6">
    <div class="text-center mb-16">
      <h2 class="text-5xl font-bold mb-6 tracking-tight">
        Real-Time Inventory Intelligence
      </h2>
      <p class="text-gray-400 text-lg max-w-2xl mx-auto leading-relaxed">
        Stop relying on outdated spreadsheets. Mercator Intelligence gives you a unified view of your entire inventory with AI-powered insights and actionable recommendations.
      </p>
    </div>

    <!-- Inventory Dashboard UI Mockup -->
    <div class="bg-white rounded-lg overflow-hidden shadow-2xl mb-20 text-gray-900 mx-auto max-w-[1000px]">
      <!-- Window Header -->
      <div class="bg-gray-50 border-b border-gray-200 px-4 py-2 flex items-center justify-between">
         <div class="flex items-center gap-2">
            <span class="text-xs font-semibold text-gray-700">Inventory Overview - Q1 2025</span>
         </div>
         <div class="flex items-center gap-3">
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>👁️</span> View
            </div>
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>📊</span> All metrics
            </div>
            <div class="flex items-center gap-1 text-xs text-gray-500 bg-white border border-gray-200 px-2 py-1 rounded">
               <span>⬇️</span> Export
            </div>
            <button class="text-gray-400 hover:text-gray-600">✕</button>
         </div>
      </div>

      <!-- Table Header -->
      <div class="grid grid-cols-12 bg-gray-50 border-b border-gray-200 text-[10px] font-bold text-gray-500 uppercase tracking-wider py-2 px-4">
         <div class="col-span-1">Status</div>
         <div class="col-span-2">SKU</div>
         <div class="col-span-3">Product Name</div>
         <div class="col-span-1">On Hand</div>
         <div class="col-span-1">On Order</div>
         <div class="col-span-2">AI Action</div>
         <div class="col-span-1">Priority</div>
         <div class="col-span-1">Category</div>
      </div>

      <!-- Table Body - Empty State / Search for effect -->
      <div class="h-[400px] bg-white relative">
         <!-- Search Overlay Effect -->
         <div class="absolute top-4 left-4 right-4 bg-white border border-gray-200 shadow-sm rounded p-2 flex items-center gap-2 max-w-md z-10">
            <span class="text-gray-400">🔍</span>
            <span class="text-sm text-gray-900">Winter|</span>
            <div class="w-[1px] h-4 bg-primary-500 animate-pulse"></div>
         </div>
         
         <!-- Blurred/Faded rows to simulate content behind search -->
         <div class="opacity-30 pointer-events-none">
             {#each Array(8) as _, i}
             <div class="grid grid-cols-12 border-b border-gray-100 py-3 px-4 text-xs text-gray-600">
                <div class="col-span-1 flex items-center">
                   {#if i === 0}
                      <div class="w-2 h-2 rounded-full bg-red-500 mr-2"></div>
                   {:else if i === 1}
                      <div class="w-2 h-2 rounded-full bg-yellow-500 mr-2"></div>
                   {:else}
                      <div class="w-2 h-2 rounded-full bg-green-500 mr-2"></div>
                   {/if}
                </div>
                <div class="col-span-2 font-mono">SKU-{8000 + i * 100}</div>
                <div class="col-span-3">Product Item {i + 1}</div>
                <div class="col-span-1">{Math.floor(Math.random() * 500) + 100}</div>
                <div class="col-span-1">{Math.floor(Math.random() * 200)}</div>
                <div class="col-span-2 text-primary-600">Reorder +{Math.floor(Math.random() * 300) + 50}</div>
                <div class="col-span-1">{i === 0 ? 'High' : i === 1 ? 'Med' : 'Low'}</div>
                <div class="col-span-1">Apparel</div>
             </div>
             {/each}
         </div>
      </div>
    </div>

    <!-- Features Grid -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-x-12 gap-y-16 text-left">
       <!-- Feature 1 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/><polyline points="3.27 6.96 12 12.01 20.73 6.96"/><line x1="12" y1="22.08" x2="12" y2="12"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Demand Forecasting</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             AI-powered predictions analyze historical sales, seasonality, and market trends to forecast demand with unprecedented accuracy.
          </p>
       </div>

       <!-- Feature 2 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"/><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Automated Reorder Points</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Dynamic reorder points that adjust based on lead times, demand variability, and service level targets—no manual updates needed.
          </p>
       </div>

       <!-- Feature 3 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21.5 2v6h-6"/><path d="M2.5 22v-6h6"/><path d="M2 11.5a10 10 0 0 1 18.8-4.3L21.5 8"/><path d="M22 12.5a10 10 0 0 1-18.8 4.2L2.5 16"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Multi-Location Optimization</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Optimize inventory across all warehouses and stores. Automatically balance stock levels to minimize costs while meeting demand.
          </p>
       </div>

       <!-- Feature 4 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 9h16"/><path d="M4 15h16"/><path d="M10 3L8 21"/><path d="M16 3l-2 18"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Supplier Performance</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Track supplier lead times, reliability, and quality. Get alerts when supplier performance impacts your inventory decisions.
          </p>
       </div>

       <!-- Feature 5 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Real-Time Alerts</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             Instant notifications for stockouts, overstock situations, and critical inventory events—stay ahead of problems before they impact sales.
          </p>
       </div>

       <!-- Feature 6 -->
       <div>
          <div class="flex items-center gap-3 mb-3">
             <div class="text-gray-400">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="4" width="6" height="6" rx="1"/><rect x="14" y="4" width="6" height="6" rx="1"/><rect x="4" y="14" width="6" height="6" rx="1"/><path d="M14 17h6"/></svg>
             </div>
             <h3 class="text-lg font-bold text-white">Category Intelligence</h3>
          </div>
          <p class="text-sm text-gray-400 leading-relaxed">
             AI learns category-specific patterns and behaviors. Apparel, electronics, groceries—each gets tailored inventory strategies.
          </p>
       </div>
    </div>
  </div>
</section>
