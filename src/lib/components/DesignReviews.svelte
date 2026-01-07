<script>
  let activeTab = 'Planning';
  const tabs = ['Planning', 'Ordering', 'Receiving', 'Allocation'];
</script>

<section class="py-24 bg-white text-center">
  <div class="max-w-[1200px] mx-auto px-6">
    <h2 class="text-5xl font-bold mb-6 tracking-tight text-gray-900">
      Built Into Your<br>Actual Workflows
    </h2>
    
    <!-- Tabs -->
    <div class="flex justify-center mb-8">
      <div class="bg-gray-100 p-1 rounded-lg inline-flex">
        {#each tabs as tab}
          <button 
            class="px-4 py-1.5 text-sm font-medium rounded-md transition-all {activeTab === tab ? 'bg-white text-gray-900 shadow-sm' : 'text-gray-500 hover:text-gray-700'}"
            on:click={() => activeTab = tab}
          >
            {tab}
          </button>
        {/each}
      </div>
    </div>

    <p class="text-lg text-gray-600 mb-16 max-w-2xl mx-auto leading-relaxed">
      Mercator Intelligence integrates directly into your planning, ordering, and allocation processes.<br>
      Get AI recommendations exactly when and where you need them.
    </p>

    <!-- UI Mockup -->
    <div class="bg-white rounded-xl shadow-2xl overflow-hidden border border-gray-200 text-left h-[700px] flex flex-col">
      <!-- Toolbar -->
      <div class="h-12 border-b border-gray-200 flex items-center justify-between px-4 bg-white">
        <div class="flex items-center gap-4">
           <span class="text-xs font-mono text-gray-500">Purchase Order #PO-2847</span>
           <span class="text-gray-300">/</span>
           <span class="text-xs font-bold text-gray-900 flex items-center gap-2">
             <span class="w-2 h-2 rounded-full bg-primary-500"></span>
             Winter Collection - Q1 2025
           </span>
        </div>
        
        <div class="flex items-center gap-6">
           <div class="flex items-center gap-4 text-xs font-medium text-gray-500">
              <button class="hover:text-gray-900 flex items-center gap-1"><span>📊</span> Analytics</button>
              <button class="text-primary-600 flex items-center gap-1 border-b-2 border-primary-500 pb-3 mt-3"><span>🤖</span> AI Insights <span class="bg-primary-100 text-primary-600 px-1 rounded text-[10px]">8</span></button>
              <button class="hover:text-gray-900 flex items-center gap-1"><span>📋</span> History</button>
           </div>
        </div>

        <div class="flex items-center gap-2">
           <button class="text-xs border border-gray-200 rounded px-2 py-1 flex items-center gap-1 text-gray-600">Filter ▼</button>
           <button class="text-xs border border-gray-200 rounded px-2 py-1 flex items-center gap-1 text-gray-600">Export ▼</button>
        </div>
      </div>

      <div class="flex flex-1 overflow-hidden">
        <!-- Left Sidebar (Categories) -->
        <div class="w-64 bg-gray-50 border-r border-gray-200 flex flex-col text-xs">
           <div class="p-2 border-b border-gray-200 flex items-center justify-between">
              <span class="font-bold text-gray-700">CATEGORIES</span>
              <div class="flex gap-1 text-gray-400">
                 <span>🔍</span>
                 <span>⚙️</span>
              </div>
           </div>
           <div class="flex-1 overflow-y-auto p-2 space-y-1">
              <div class="flex items-center gap-2 text-gray-600 pl-2">
                 <span>▼</span> <span>All Products</span>
              </div>
              <div class="flex items-center gap-2 text-gray-600 pl-2">
                 <span>▼</span> <span>Apparel</span>
              </div>
              <div class="flex items-center gap-2 font-medium text-gray-900 pl-2 bg-primary-50 rounded py-1">
                 <span>▼</span> <span>Winter Collection</span> <span class="ml-auto text-[10px] bg-primary-200 px-1 rounded text-primary-700">142 SKUs</span>
              </div>
              <div class="pl-6 space-y-1">
                 <div class="flex items-center gap-2 text-gray-700">
                    <span>📦</span> <span>Jackets</span> <span class="ml-auto text-[10px] bg-gray-200 px-1 rounded text-gray-600">48</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-700">
                    <span>📦</span> <span>Sweaters</span> <span class="ml-auto text-[10px] bg-gray-200 px-1 rounded text-gray-600">36</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-500">
                    <span>📦</span> <span>Boots</span> <span class="ml-auto text-[10px] bg-gray-200 px-1 rounded text-gray-600">28</span>
                 </div>
                 <div class="flex items-center gap-2 text-gray-500">
                    <span>📦</span> <span>Accessories</span> <span class="ml-auto text-[10px] bg-gray-200 px-1 rounded text-gray-600">30</span>
                 </div>
              </div>
              <div class="flex items-center gap-2 text-gray-600 pl-2 pt-2">
                 <span>▶</span> <span>Spring Collection</span> <span class="ml-auto text-[10px] bg-gray-200 px-1 rounded text-gray-600">89</span>
              </div>
              <div class="flex items-center gap-2 text-gray-600 pl-2">
                 <span>▶</span> <span>Footwear</span>
              </div>
           </div>
        </div>

        <!-- Center (Workflow View) -->
        <div class="flex-1 bg-white relative overflow-hidden">
           <!-- Image with overlay -->
           <div class="absolute inset-0">
              <img src="/generated/image-retail-operations-manager-reviewing-data-1767814298621-1.webp" alt="Retail operations" class="w-full h-full object-cover opacity-20" />
           </div>
           
           <!-- Workflow cards overlay -->
           <div class="relative z-10 p-8 flex flex-col gap-4 h-full justify-center">
              <!-- Workflow Step 1 -->
              <div class="bg-white rounded-lg shadow-lg p-4 border-l-4 border-primary-500 max-w-md">
                 <div class="flex items-center gap-3 mb-2">
                    <div class="w-8 h-8 rounded-full bg-primary-100 text-primary-600 flex items-center justify-center font-bold text-sm">1</div>
                    <div>
                       <div class="text-sm font-bold text-gray-900">Planning Phase</div>
                       <div class="text-xs text-gray-500">AI analyzes demand patterns</div>
                    </div>
                 </div>
                 <div class="text-xs text-gray-600 bg-primary-50 p-2 rounded">
                    Forecast shows 18% increase in jacket demand for next quarter
                 </div>
              </div>

              <!-- Workflow Step 2 -->
              <div class="bg-white rounded-lg shadow-lg p-4 border-l-4 border-blue-500 max-w-md ml-12">
                 <div class="flex items-center gap-3 mb-2">
                    <div class="w-8 h-8 rounded-full bg-blue-100 text-blue-600 flex items-center justify-center font-bold text-sm">2</div>
                    <div>
                       <div class="text-sm font-bold text-gray-900">Order Optimization</div>
                       <div class="text-xs text-gray-500">Recommendations generated</div>
                    </div>
                 </div>
                 <div class="text-xs text-gray-600 bg-blue-50 p-2 rounded">
                    Suggested order: 2,450 units across 48 SKUs
                 </div>
              </div>

              <!-- Workflow Step 3 -->
              <div class="bg-white rounded-lg shadow-lg p-4 border-l-4 border-green-500 max-w-md ml-24">
                 <div class="flex items-center gap-3 mb-2">
                    <div class="w-8 h-8 rounded-full bg-green-100 text-green-600 flex items-center justify-center font-bold text-sm">3</div>
                    <div>
                       <div class="text-sm font-bold text-gray-900">Approval & Execution</div>
                       <div class="text-xs text-gray-500">One-click to execute</div>
                    </div>
                 </div>
                 <div class="text-xs text-gray-600 bg-green-50 p-2 rounded">
                    Review and approve orders directly in your workflow
                 </div>
              </div>
           </div>
           
           <!-- User Avatars overlay -->
           <div class="absolute top-4 left-1/2 transform -translate-x-1/2 bg-white/90 backdrop-blur rounded-full px-3 py-1 flex items-center gap-2 text-xs shadow-sm">
              <div class="flex -space-x-2">
                 <div class="w-6 h-6 rounded-full bg-primary-500 border-2 border-white"></div>
                 <div class="w-6 h-6 rounded-full bg-blue-500 border-2 border-white"></div>
                 <div class="w-6 h-6 rounded-full bg-green-500 border-2 border-white"></div>
              </div>
              <span class="text-gray-600">Team collaborating</span>
           </div>
        </div>

        <!-- Right Sidebar (AI Insights) -->
        <div class="w-80 bg-white border-l border-gray-200 flex flex-col">
           <div class="p-4 border-b border-gray-100">
              <div class="flex items-center gap-2 mb-3">
                 <div class="w-6 h-6 rounded-full bg-primary-100 text-primary-600 flex items-center justify-center text-xs">🤖</div>
                 <input type="text" placeholder="Ask AI about inventory..." class="flex-1 bg-transparent text-sm focus:outline-none">
              </div>
              <div class="flex justify-between items-center">
                 <div class="flex gap-2 text-gray-400">
                    <button>📊</button>
                    <button>📈</button>
                    <button>💡</button>
                 </div>
                 <button class="bg-gray-900 text-white text-xs px-3 py-1.5 rounded font-medium">Ask</button>
              </div>
           </div>
           
           <div class="flex-1 overflow-y-auto p-4 space-y-6">
              <div class="flex items-center justify-between text-[10px] font-bold text-gray-400 uppercase tracking-wider mb-2">
                 <span>AI Insights</span>
                 <div class="flex gap-2">
                    <button>Filter</button>
                    <button>Sort</button>
                 </div>
              </div>

              <!-- Insight 1 -->
              <div class="flex gap-3">
                 <div class="w-8 h-8 rounded-full bg-primary-100 flex-shrink-0 flex items-center justify-center text-xs">🎯</div>
                 <div>
                    <div class="flex items-baseline gap-2 mb-1">
                       <span class="text-xs font-bold text-gray-900">High Priority Alert</span>
                       <span class="text-[10px] text-gray-400">2h</span>
                    </div>
                    <div class="text-xs text-gray-600 bg-primary-50 p-2 rounded-lg border border-primary-100 mb-1">
                       Winter jacket demand up 23% vs forecast. Recommend increasing order by 850 units to avoid stockout.
                    </div>
                    <div class="flex items-center gap-2 mt-1">
                       <button class="text-[10px] text-primary-600 hover:underline">Apply recommendation</button>
                    </div>
                 </div>
              </div>

              <!-- Insight 2 -->
              <div class="flex gap-3">
                 <div class="w-8 h-8 rounded-full bg-yellow-100 flex-shrink-0 flex items-center justify-center text-xs">⚠️</div>
                 <div>
                    <div class="flex items-baseline gap-2 mb-1">
                       <span class="text-xs font-bold text-gray-900">Supplier Update</span>
                       <span class="text-[10px] text-gray-400">4h</span>
                    </div>
                    <div class="text-xs text-gray-600 mb-1">
                       Lead time for Supplier A extended by 2 weeks. Adjust safety stock for 12 affected SKUs.
                    </div>
                    <div class="flex items-center gap-2 mt-1">
                       <button class="text-[10px] text-gray-600 hover:underline">View details</button>
                    </div>
                 </div>
              </div>

              <!-- Insight 3 -->
              <div class="flex gap-3">
                 <div class="w-8 h-8 rounded-full bg-green-100 flex-shrink-0 flex items-center justify-center text-xs">✓</div>
                 <div>
                    <div class="flex items-baseline gap-2 mb-1">
                       <span class="text-xs font-bold text-gray-900">Optimization Complete</span>
                       <span class="text-[10px] text-gray-400">1d</span>
                    </div>
                    <div class="text-xs text-gray-600 mb-1">
                       Successfully optimized 48 SKUs. Projected inventory cost reduction: $12,400/month.
                    </div>
                 </div>
              </div>
           </div>
        </div>
      </div>
    </div>
  </div>
</section>
