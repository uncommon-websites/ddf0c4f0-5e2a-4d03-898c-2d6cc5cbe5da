<script>
</script>

<section class="bg-gray-900 text-white py-24 overflow-hidden relative">
  <!-- Background gradient effect -->
  <div class="absolute inset-0 bg-gradient-to-b from-gray-800 to-gray-950 opacity-100"></div>
  
  <div class="relative max-w-[1200px] mx-auto px-6 text-center">
    <h2 class="text-5xl font-bold mb-6 tracking-tight leading-tight">
      AI That Understands<br>Your Inventory
    </h2>
    <p class="text-gray-300 text-lg max-w-2xl mx-auto mb-16 leading-relaxed">
      Mercator Intelligence analyzes demand patterns, supply constraints, and business context to deliver actionable inventory recommendations—all within your existing workflows.
    </p>

    <!-- UI Mockup -->
    <div class="bg-white rounded-xl shadow-2xl overflow-hidden text-left text-gray-900 mx-auto max-w-[1000px] border border-gray-700/30">
      <!-- Window Controls -->
      <div class="bg-gray-50 border-b border-gray-200 px-4 py-3 flex items-center gap-2">
        <div class="flex gap-1.5">
          <div class="w-3 h-3 rounded-full bg-red-400"></div>
          <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
          <div class="w-3 h-3 rounded-full bg-green-400"></div>
        </div>
        <div class="ml-4 flex items-center gap-2 text-xs font-medium text-gray-600 bg-white px-2 py-1 rounded border border-gray-200 shadow-sm">
           <span class="w-3 h-3 bg-primary-600 rounded-full flex items-center justify-center text-[8px] text-white">M</span>
           Inventory Dashboard
           <span class="text-gray-400">▼</span>
        </div>
      </div>

      <div class="flex h-[500px]">
        <!-- Sidebar -->
        <div class="w-48 bg-gray-50 border-r border-gray-200 p-3 flex flex-col gap-1">
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
            <span class="opacity-70">📊</span> Overview
          </div>
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-900 bg-white shadow-sm border border-gray-200 rounded cursor-pointer">
            <span class="opacity-70">🎯</span> Actions
          </div>
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
            <span class="opacity-70">📦</span> Stock Levels
          </div>
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
            <span class="opacity-70">📈</span> Demand Forecast
          </div>
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
            <span class="opacity-70">🚚</span> Suppliers
          </div>
          <div class="flex items-center gap-2 px-2 py-1.5 text-xs font-medium text-gray-600 hover:bg-gray-200 rounded cursor-pointer">
            <span class="opacity-70">⚡</span> Alerts
          </div>
          
          <div class="mt-auto text-[10px] text-gray-400 px-2">2,847 SKUs</div>
        </div>

        <!-- Main List -->
        <div class="flex-1 bg-white flex flex-col">
          <div class="border-b border-gray-100 p-3">
             <div class="relative">
                <span class="absolute left-2 top-1.5 text-gray-400 text-xs">🔍</span>
                <input type="text" placeholder="Search SKUs and products..." class="w-full bg-gray-50 border border-gray-200 rounded pl-7 pr-3 py-1 text-xs focus:outline-none focus:border-primary-500">
             </div>
          </div>
          <div class="flex-1 overflow-y-auto">
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 hover:bg-primary-50 cursor-pointer group">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-red-100 text-red-600 rounded flex items-center justify-center text-[8px]">⚠️</div>
                   <span class="text-xs font-medium text-gray-700">Reorder Now</span>
                </div>
                <div class="text-[10px] text-gray-400 group-hover:text-primary-600">24 SKUs</div>
             </div>
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 bg-primary-50/50 cursor-pointer">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-primary-100 text-primary-600 rounded flex items-center justify-center text-[8px]">🎯</div>
                   <span class="text-xs font-medium text-gray-900">Review Quantities</span>
                </div>
                <div class="text-[10px] text-gray-400">18 SKUs</div>
             </div>
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 hover:bg-primary-50 cursor-pointer group">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-yellow-100 text-yellow-600 rounded flex items-center justify-center text-[8px]">⏸️</div>
                   <span class="text-xs font-medium text-gray-700">Hold Orders</span>
                </div>
                <div class="text-[10px] text-gray-400 group-hover:text-primary-600">7 SKUs</div>
             </div>
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 hover:bg-primary-50 cursor-pointer group">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-blue-100 text-blue-600 rounded flex items-center justify-center text-[8px]">📊</div>
                   <span class="text-xs font-medium text-gray-700">Optimize Safety Stock</span>
                </div>
                <div class="text-[10px] text-gray-400 group-hover:text-primary-600">31 SKUs</div>
             </div>
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 hover:bg-primary-50 cursor-pointer group">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-green-100 text-green-600 rounded flex items-center justify-center text-[8px]">✓</div>
                   <span class="text-xs font-medium text-gray-700">All Good</span>
                </div>
                <div class="text-[10px] text-gray-400 group-hover:text-primary-600">2,767 SKUs</div>
             </div>
             <div class="flex items-center justify-between px-4 py-2 border-b border-gray-50 hover:bg-primary-50 cursor-pointer group">
                <div class="flex items-center gap-2">
                   <div class="w-4 h-4 bg-gray-200 rounded flex items-center justify-center text-[8px]">📦</div>
                   <span class="text-xs font-medium text-gray-700">Slow Movers</span>
                </div>
             </div>
          </div>
        </div>

        <!-- Right Panel -->
        <div class="w-80 bg-white border-l border-gray-200 flex flex-col">
          <div class="p-3 border-b border-gray-100 flex justify-between items-center">
             <span class="text-[10px] font-bold text-gray-400 uppercase tracking-wider">AI Recommendation</span>
             <button class="text-[10px] border border-gray-200 rounded px-2 py-1 hover:bg-gray-50 flex items-center gap-1">
                <span>🤖</span> View Details
             </button>
          </div>
          
          <div class="p-4 flex-1 overflow-y-auto">
             <div class="text-[10px] font-bold text-gray-400 uppercase tracking-wider mb-2">Review Quantities</div>
             
             <!-- Action Item -->
             <div class="mb-4 relative pl-4 border-l-2 border-primary-500">
                <div class="absolute -left-[5px] top-0 w-2 h-2 rounded-full bg-primary-500"></div>
                <div class="flex justify-between items-start mb-1">
                   <span class="text-xs font-bold text-gray-900">SKU-8472: Winter Jacket</span>
                   <span class="text-[10px] text-gray-400">High Priority</span>
                </div>
                <div class="text-[10px] text-gray-600 mb-2">
                   Demand forecast shows 23% increase vs. last year. Current order quantity may lead to stockout by Week 3.
                </div>
                <span class="inline-block px-1.5 py-0.5 bg-primary-100 text-primary-700 text-[9px] rounded font-medium">Increase by 850 units</span>
             </div>

             <!-- Action Item -->
             <div class="mb-4 relative pl-4 border-l-2 border-gray-200">
                <div class="absolute -left-[5px] top-0 w-2 h-2 rounded-full bg-yellow-500"></div>
                <div class="flex justify-between items-start mb-1">
                   <span class="text-xs font-bold text-gray-900">SKU-3291: Running Shoes</span>
                   <span class="text-[10px] text-gray-400">Medium Priority</span>
                </div>
                <div class="text-[10px] text-gray-600 mb-2">
                   Supplier lead time extended by 2 weeks. Adjust safety stock to maintain service level.
                </div>
                <span class="inline-block px-1.5 py-0.5 bg-yellow-100 text-yellow-700 text-[9px] rounded font-medium">Add 320 units buffer</span>
             </div>

             <div class="flex items-center gap-2 mb-4 pl-4">
                <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
                <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
                <div class="w-1 h-1 bg-gray-300 rounded-full"></div>
                <span class="text-[10px] text-gray-400">Show 16 more actions</span>
             </div>

             <!-- Action Item -->
             <div class="mb-4 relative pl-4 border-l-2 border-gray-200">
                <div class="absolute -left-[5px] top-0 w-2 h-2 rounded-full bg-gray-300"></div>
                <div class="flex justify-between items-start mb-1">
                   <span class="text-xs font-bold text-gray-500">SKU-1847: Summer Dress</span>
                   <span class="text-[10px] text-gray-400">Low Priority</span>
                </div>
                <div class="text-[10px] text-gray-500">
                   Seasonal trend ending. Consider reducing next order by 15% based on historical patterns.
                </div>
             </div>
             
             <!-- Action Item -->
             <div class="mb-4 relative pl-4 border-l-2 border-gray-200">
                <div class="absolute -left-[5px] top-0 w-2 h-2 rounded-full bg-gray-300"></div>
                <div class="flex justify-between items-start mb-1">
                   <span class="text-xs font-bold text-gray-500">SKU-9124: Backpack</span>
                   <span class="text-[10px] text-gray-400">Reviewed</span>
                </div>
                <div class="text-[10px] text-gray-500">
                   Order quantity aligned with demand. No action needed at this time.
                </div>
             </div>
          </div>
          
          <div class="p-3 border-t border-gray-100 bg-gray-50 flex justify-between items-center">
             <div class="flex items-center gap-2 text-[10px] text-gray-500">
                <button class="hover:text-gray-900">✕</button>
                <span>Dismiss all</span>
             </div>
             <div class="flex gap-2">
                <button class="bg-white border border-gray-200 text-gray-700 text-[10px] px-2 py-1 rounded hover:bg-gray-50">Export</button>
                <button class="bg-gray-900 text-white text-[10px] px-2 py-1 rounded hover:bg-gray-800">Apply Actions</button>
             </div>
          </div>
        </div>
      </div>
    </div>
    
    <!-- Bottom Integration Info -->
    <div class="mt-12 flex items-center justify-center gap-4 bg-gray-950 rounded-lg p-4 max-w-4xl mx-auto border border-gray-800">
       <div class="flex items-center gap-4 border-r border-gray-700 pr-4">
          <div class="w-8 h-8 bg-white rounded flex items-center justify-center font-bold text-black text-xs">ERP</div>
          <div class="w-8 h-8 bg-blue-600 rounded flex items-center justify-center font-bold text-white text-xs">WMS</div>
          <div class="w-8 h-8 bg-green-600 rounded flex items-center justify-center font-bold text-white text-xs">POS</div>
       </div>
       <p class="text-xs text-gray-400 text-left flex-1">
          Mercator Intelligence integrates seamlessly with your existing systems. Connect to your ERP, WMS, and POS platforms to get AI-driven recommendations without disrupting your workflows.
       </p>
       <button class="bg-gray-800 text-white px-3 py-1.5 rounded text-xs font-semibold hover:bg-gray-700">Request Demo</button>
    </div>
  </div>
</section>
