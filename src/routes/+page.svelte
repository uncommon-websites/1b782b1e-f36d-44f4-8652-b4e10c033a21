<script>
    import Navbar from '$lib/components/Navbar.svelte';
    import Footer from '$lib/components/Footer.svelte';
    import FeatureRow from '$lib/components/FeatureRow.svelte';
</script>

<div class="bg-[var(--color-dark)] min-h-screen flex flex-col">
    <Navbar />

    <main class="flex-grow">
        <!-- Hero Section -->
        <section class="relative pt-32 pb-20 overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="max-w-4xl mx-auto text-center">
                    <!-- Search/Notification Pill -->
                    <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-sm border border-white/10 rounded-full px-4 py-1.5 mb-8">
                        <span class="w-2 h-2 rounded-full bg-[var(--color-primary)]"></span>
                        <span class="text-white text-sm font-medium">Zero Seller Fees</span>
                        <span class="text-gray-400 text-sm">Forever</span>
                        <svg class="w-4 h-4 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                    </div>

                    <h1 class="text-5xl md:text-7xl font-bold text-white tracking-tight mb-6 text-balance">
                        Buy and sell precious metals with confidence.
                    </h1>
                    
                    <p class="text-lg md:text-xl text-gray-400 mb-10 max-w-2xl mx-auto leading-relaxed text-balance">
                        Connect with verified dealers offering gold, silver, platinum, and rare coins. Transparent spot-linked pricing, zero seller fees, and nationwide shipping. Your trusted marketplace for precious metals.
                    </p>
                    
                    <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                        <button class="bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Browse Marketplace
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </button>
                        <button class="bg-transparent border border-white/20 hover:bg-white/10 text-white px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2">
                            Become a Dealer
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14M12 5l7 7-7 7"/>
                            </svg>
                        </button>
                    </div>
                </div>
            </div>

            <!-- Hero Images/Cards -->
            <div class="mt-20 relative">
                <div class="flex justify-center gap-6 overflow-hidden px-6">
                    <!-- Card 1 - Gold Coin Listing -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform -rotate-2 mt-8">
                        <div class="bg-white p-6">
                            <div class="flex items-center justify-between mb-4">
                                <div class="text-xs font-semibold text-gray-500 uppercase">American Gold Eagle</div>
                                <div class="px-3 py-1 bg-[var(--color-primary)]/10 rounded-full text-[var(--color-primary)] text-sm font-bold">$4,308.39</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-32 bg-gradient-to-br from-yellow-100 to-yellow-200 rounded-lg w-full flex items-center justify-center">
                                    <div class="w-24 h-24 rounded-full bg-gradient-to-br from-yellow-400 to-yellow-600 shadow-lg"></div>
                                </div>
                                <div class="flex items-center justify-between text-sm">
                                    <span class="text-gray-600">1 oz • 2025</span>
                                    <span class="text-green-600 font-medium flex items-center gap-1">
                                        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                                        Verified Dealer
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 2 (Center) - Live Pricing -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 z-10">
                        <div class="bg-white h-full flex flex-col">
                            <div class="bg-gradient-to-br from-[var(--color-primary)] to-[var(--color-primary-dark)] p-6">
                                <div class="flex justify-between items-center">
                                    <div class="text-white font-bold text-lg">Live Spot Prices</div>
                                    <div class="w-2 h-2 rounded-full bg-white animate-pulse"></div>
                                </div>
                            </div>
                            <div class="p-6 flex-grow space-y-4">
                                <div class="flex justify-between items-center pb-3 border-b border-gray-100">
                                    <div class="flex items-center gap-2">
                                        <div class="w-8 h-8 rounded-full bg-yellow-400"></div>
                                        <span class="font-semibold">Gold</span>
                                    </div>
                                    <div class="text-right">
                                        <div class="font-bold text-lg">$4,308.39</div>
                                        <div class="text-xs text-green-600">+2.4%</div>
                                    </div>
                                </div>
                                <div class="flex justify-between items-center pb-3 border-b border-gray-100">
                                    <div class="flex items-center gap-2">
                                        <div class="w-8 h-8 rounded-full bg-gray-300"></div>
                                        <span class="font-semibold">Silver</span>
                                    </div>
                                    <div class="text-right">
                                        <div class="font-bold text-lg">$63.05</div>
                                        <div class="text-xs text-green-600">+1.8%</div>
                                    </div>
                                </div>
                                <div class="flex justify-between items-center">
                                    <div class="flex items-center gap-2">
                                        <div class="w-8 h-8 rounded-full bg-gray-400"></div>
                                        <span class="font-semibold">Platinum</span>
                                    </div>
                                    <div class="text-right">
                                        <div class="font-bold text-lg">$1,751.22</div>
                                        <div class="text-xs text-red-600">-0.5%</div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Card 3 - Silver Coin Listing -->
                    <div class="w-[350px] md:w-[450px] flex-shrink-0 rounded-xl overflow-hidden shadow-2xl border border-white/10 transform rotate-2 mt-8">
                        <div class="bg-white p-6">
                            <div class="flex items-center justify-between mb-4">
                                <div class="text-xs font-semibold text-gray-500 uppercase">Canadian Maple Leaf</div>
                                <div class="px-3 py-1 bg-[var(--color-primary)]/10 rounded-full text-[var(--color-primary)] text-sm font-bold">$72.35</div>
                            </div>
                            <div class="space-y-3">
                                <div class="h-32 bg-gradient-to-br from-gray-100 to-gray-200 rounded-lg w-full flex items-center justify-center">
                                    <div class="w-24 h-24 rounded-full bg-gradient-to-br from-gray-300 to-gray-400 shadow-lg"></div>
                                </div>
                                <div class="flex items-center justify-between text-sm">
                                    <span class="text-gray-600">1 oz Silver • 2024</span>
                                    <span class="text-green-600 font-medium flex items-center gap-1">
                                        <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                                        Verified Dealer
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Trust Indicators Section -->
        <section class="py-16 border-y border-white/5 bg-black/20">
            <div class="container mx-auto px-6">
                <p class="text-center text-gray-400 mb-8 text-sm">Trusted by collectors and dealers nationwide</p>
                <div class="flex flex-wrap justify-center items-center gap-12 md:gap-16">
                    <div class="flex flex-col items-center text-center">
                        <div class="text-3xl md:text-4xl font-bold text-white mb-1">1,000+</div>
                        <div class="text-sm text-gray-400">Listed Items</div>
                    </div>
                    <div class="flex flex-col items-center text-center">
                        <div class="text-3xl md:text-4xl font-bold text-white mb-1">50</div>
                        <div class="text-sm text-gray-400">States Served</div>
                    </div>
                    <div class="flex flex-col items-center text-center">
                        <div class="text-3xl md:text-4xl font-bold text-white mb-1">$0</div>
                        <div class="text-sm text-gray-400">Seller Fees</div>
                    </div>
                    <div class="flex flex-col items-center text-center">
                        <div class="text-3xl md:text-4xl font-bold text-white mb-1">100%</div>
                        <div class="text-sm text-gray-400">Verified Dealers</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Why Choose Us Section -->
        <section class="py-32 relative overflow-hidden">
            <div class="container mx-auto px-6 relative z-10">
                <div class="text-center mb-24">
                    <h2 class="text-[var(--color-primary)] font-mono text-xs tracking-[0.2em] uppercase mb-6">Why Lone Star Coins</h2>
                    <h3 class="text-4xl md:text-6xl font-bold text-white mb-2 tracking-tight">A precious metals marketplace.</h3>
                    <h3 class="text-4xl md:text-6xl font-bold text-gray-600 tracking-tight">Built on trust.</h3>
                </div>

                <div class="grid md:grid-cols-2 gap-16 items-center max-w-6xl mx-auto">
                    <!-- Visual Card -->
                    <div class="bg-gradient-to-br from-gray-800 to-gray-900 rounded-3xl p-12 aspect-[4/3] relative overflow-hidden flex items-center justify-center shadow-2xl border border-white/10">
                        <!-- Coin Stacks Visual -->
                        <div class="relative z-10 w-full max-w-[320px]">
                            <!-- Gold Coin Stack -->
                            <div class="bg-gradient-to-br from-yellow-400 to-yellow-600 rounded-2xl p-6 mb-6 shadow-xl relative overflow-hidden group hover:scale-105 transition-transform duration-500">
                                <div class="flex items-center justify-between mb-4">
                                    <div class="text-yellow-900 font-bold text-lg">Gold</div>
                                    <div class="text-yellow-900 font-mono text-sm">$4,308.39/oz</div>
                                </div>
                                <div class="flex gap-2">
                                    <div class="w-12 h-12 rounded-full bg-yellow-500 shadow-lg"></div>
                                    <div class="w-12 h-12 rounded-full bg-yellow-500 shadow-lg -ml-6"></div>
                                    <div class="w-12 h-12 rounded-full bg-yellow-500 shadow-lg -ml-6"></div>
                                </div>
                            </div>
                            
                            <!-- Floating Pills -->
                            <div class="relative">
                                <div class="absolute -left-4 top-0 bg-white text-black px-5 py-2.5 rounded-full text-sm font-semibold shadow-lg flex items-center gap-2 transform -rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-green-100 flex items-center justify-center text-green-600">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"></path></svg>
                                    </div>
                                    Verified Dealers
                                </div>
                                <div class="absolute -right-4 top-12 bg-white/10 backdrop-blur-md text-white px-5 py-2.5 rounded-full text-sm font-semibold border border-white/20 flex items-center gap-2 transform rotate-2">
                                    <div class="w-5 h-5 rounded-full bg-[var(--color-primary)]/30 flex items-center justify-center text-[var(--color-primary-light)]">
                                        <svg class="w-3 h-3" fill="currentColor" viewBox="0 0 20 20"><path d="M8.433 7.418c.155-.103.346-.196.567-.267v1.698a2.305 2.305 0 01-.567-.267C8.07 8.34 8 8.114 8 8c0-.114.07-.34.433-.582zM11 12.849v-1.698c.22.071.412.164.567.267.364.243.433.468.433.582 0 .114-.07.34-.433.582a2.305 2.305 0 01-.567.267z"></path><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm1-13a1 1 0 10-2 0v.092a4.535 4.535 0 00-1.676.662C6.602 6.234 6 7.009 6 8c0 .99.602 1.765 1.324 2.246.48.32 1.054.545 1.676.662v1.941c-.391-.127-.68-.317-.843-.504a1 1 0 10-1.51 1.31c.562.649 1.413 1.076 2.353 1.253V15a1 1 0 102 0v-.092a4.535 4.535 0 001.676-.662C13.398 13.766 14 12.991 14 12c0-.99-.602-1.765-1.324-2.246A4.535 4.535 0 0011 9.092V7.151c.391.127.68.317.843.504a1 1 0 101.511-1.31c-.563-.649-1.413-1.076-2.354-1.253V5z" clip-rule="evenodd"></path></svg>
                                    </div>
                                    Spot-Linked Pricing
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Text Content -->
                    <div class="space-y-8">
                        <h3 class="text-4xl md:text-5xl font-bold text-white tracking-tight">Trade with confidence.</h3>
                        <p class="text-gray-400 text-lg leading-relaxed max-w-lg">
                            Every dealer is verified. Every price is transparent. Every transaction is secure. Lone Star Coins brings trust and simplicity to precious metals trading.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- White Section -->
        <div class="bg-[#F9FAFB] text-black rounded-t-[4rem] relative z-20 mt-[-2rem] pt-32 pb-32">
            <div class="container mx-auto px-6">
                <!-- Header -->
                <div class="max-w-4xl mb-24">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="h-px w-12 bg-gray-300"></div>
                        <span class="text-gray-500 font-mono text-xs tracking-[0.2em] uppercase">Marketplace Features</span>
                    </div>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-900 mb-2 tracking-tight">Everything you need to buy and sell precious metals.</h2>
                    <h2 class="text-4xl md:text-6xl font-bold text-gray-400 tracking-tight mb-8">With complete confidence.</h2>
                    
                    <a href="#" class="inline-flex items-center gap-2 text-sm font-semibold border-b border-black pb-0.5 hover:text-gray-600 transition-colors">
                        Browse the marketplace
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </a>
                </div>

                <!-- Features Grid -->
                <div class="flex flex-col lg:flex-row gap-12">
                    <!-- Sidebar Navigation (Sticky) -->
                    <div class="hidden lg:block w-64 flex-shrink-0">
                        <div class="sticky top-32 space-y-4">
                            <div class="flex items-center gap-2 text-sm font-semibold text-black border-l-2 border-black pl-4 py-1">
                                <span class="w-1.5 h-1.5 rounded-full bg-[var(--color-primary)]"></span>
                                Verified Dealers
                            </div>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Spot-Linked Pricing</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Zero Seller Fees</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Secure Transactions</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Nationwide Shipping</a>
                            <a href="#" class="block text-sm text-gray-500 pl-4 py-1 hover:text-black border-l-2 border-transparent hover:border-gray-200 transition-colors">Expert Support</a>
                        </div>
                    </div>

                    <!-- Feature Cards -->
                    <div class="flex-grow space-y-8">
                        <FeatureRow 
                            title="Verified Dealers" 
                            description="Trade with confidence. Every dealer on Lone Star Coins goes through rigorous verification to ensure authenticity and trustworthiness."
                            icon="lock"
                            image="collateral"
                        />
                         <FeatureRow 
                            title="Spot-Linked Pricing" 
                            description="Always transparent. Bullion prices automatically adjust based on live spot prices for gold, silver, platinum, and palladium—no hidden markups."
                            icon="data"
                            image="data"
                        />
                         <FeatureRow 
                            title="Zero Seller Fees" 
                            description="Keep more profit. Unlike other marketplaces, we charge zero fees to sellers. List unlimited inventory and grow your business without restrictions."
                            icon="connect"
                            image="connect"
                        />
                         <FeatureRow 
                            title="Secure Transactions" 
                            description="Protected every step. Advanced security measures and buyer protection ensure safe transactions for both collectors and dealers."
                            icon="guard"
                            image="guard"
                        />
                         <FeatureRow 
                            title="Nationwide Shipping" 
                            description="Reach all 50 states. Fully insured shipping options connect dealers with collectors across the entire United States."
                            icon="preview"
                            image="preview"
                        />
                         <FeatureRow 
                            title="Expert Support" 
                            description="We're here to help. Our team of precious metals experts provides guidance on pricing, authentication, and marketplace best practices."
                            icon="lab"
                            image="lab"
                        />
                    </div>
                </div>

                <!-- Dealer CTA Section -->
                <div class="mt-32 text-center max-w-4xl mx-auto mb-24">
                    <div class="w-24 h-24 mx-auto bg-gradient-to-br from-yellow-100 to-yellow-200 rounded-full flex items-center justify-center mb-8 relative">
                        <div class="absolute inset-0 bg-yellow-300/50 blur-xl rounded-full"></div>
                        <svg class="w-10 h-10 text-yellow-700 relative z-10" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                    </div>
                    <h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8 leading-tight">
                        Are you a precious metals dealer? Join our marketplace and reach thousands of collectors nationwide.
                    </h2>
                    <button class="bg-white border border-gray-200 hover:border-gray-400 text-black px-6 py-3 rounded-full font-medium transition-colors flex items-center gap-2 mx-auto">
                        Become a Verified Dealer
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>
                </div>

                <!-- Success Stories Section -->
                <div class="mb-32">
                    <p class="text-xl text-gray-500 mb-12">Hear from our dealers and collectors.</p>
                    
                    <div class="grid md:grid-cols-3 gap-6">
                        <!-- Featured Testimonial (Large) -->
                        <div class="md:col-span-2 bg-[#0A0A0A] rounded-3xl p-10 relative overflow-hidden group min-h-[400px] flex flex-col justify-end">
                            <div class="absolute inset-0 bg-gradient-to-t from-black via-black/50 to-transparent"></div>
                            <div class="absolute top-0 right-0 w-64 h-64 bg-yellow-500/10 blur-[100px] rounded-full"></div>
                            
                            <div class="relative z-10">
                                <div class="flex items-center gap-4 mb-6">
                                    <div class="w-12 h-12 rounded-full bg-yellow-400 flex items-center justify-center">
                                        <svg class="w-6 h-6 text-yellow-900" fill="currentColor" viewBox="0 0 20 20"><path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z"></path></svg>
                                    </div>
                                    <div>
                                        <div class="text-white font-bold text-lg">Texas Coin Gallery</div>
                                        <div class="text-gray-400 text-sm">Verified Dealer since 2025</div>
                                    </div>
                                </div>
                                <h3 class="text-2xl font-bold text-white mb-4 max-w-md leading-relaxed">
                                    "Zero seller fees means we can offer better prices to our customers. Lone Star Coins has transformed how we do business."
                                </h3>
                                <p class="text-gray-400 text-sm">— Michael Rodriguez, Owner</p>
                            </div>
                        </div>

                        <!-- Smaller Cards -->
                        <div class="space-y-6">
                            <!-- Card 2 -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group min-h-[190px] flex flex-col justify-between">
                                <div class="absolute inset-0 bg-gradient-to-br from-gray-800/60 to-black"></div>
                                <div class="relative z-10">
                                    <div class="flex items-center gap-3 mb-3">
                                        <div class="w-10 h-10 rounded-full bg-gray-600"></div>
                                        <div>
                                            <div class="text-white font-semibold text-sm">Sarah Chen</div>
                                            <div class="text-gray-400 text-xs">Collector</div>
                                        </div>
                                    </div>
                                    <p class="text-white text-sm leading-relaxed">"Best place to find rare coins at fair prices. The verification process gives me peace of mind."</p>
                                </div>
                            </div>
                            <!-- Card 3 -->
                            <div class="bg-[#0A0A0A] rounded-3xl p-8 relative overflow-hidden group min-h-[190px] flex flex-col justify-between">
                                <div class="absolute inset-0 bg-gradient-to-br from-gray-800/60 to-black"></div>
                                <div class="relative z-10">
                                    <div class="flex items-center gap-3 mb-3">
                                        <div class="w-10 h-10 rounded-full bg-gray-600"></div>
                                        <div>
                                            <div class="text-white font-semibold text-sm">James Patterson</div>
                                            <div class="text-gray-400 text-xs">Investor</div>
                                        </div>
                                    </div>
                                    <p class="text-white text-sm leading-relaxed">"Spot-linked pricing is a game changer. No more wondering if I'm getting a fair deal."</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Banner -->
                <div class="bg-[#0A0A0A] rounded-3xl p-12 md:p-20 relative overflow-hidden mb-32 text-center">
                    <div class="absolute inset-0 bg-[url('/grid-pattern.svg')] opacity-10"></div>
                    <div class="absolute left-0 top-0 w-64 h-64 bg-yellow-500/10 blur-[100px] rounded-full"></div>
                    <div class="absolute right-0 bottom-0 w-64 h-64 bg-gray-400/10 blur-[100px] rounded-full"></div>
                    
                    <div class="relative z-10 max-w-3xl mx-auto">
                        <h2 class="text-4xl md:text-6xl font-bold text-white mb-6 tracking-tight">
                            Start your collection. <span class="text-[var(--color-primary)]">Grow your wealth.</span>
                        </h2>
                        <p class="text-gray-400 mb-10">
                            From American Eagles to rare numismatics, discover thousands of precious metals listings from verified dealers across the United States.
                        </p>
                        <div class="inline-flex items-center gap-2 bg-white/10 backdrop-blur-md border border-white/10 rounded-full px-4 py-2 text-white text-sm hover:bg-white/20 transition-colors cursor-pointer">
                            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"></path></svg>
                            Browse Marketplace
                            <svg class="w-3 h-3" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg>
                        </div>
                    </div>
                </div>

                <!-- Product Categories -->
                <div class="text-center mb-32">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                        Gold. Silver. Platinum. Palladium.<br>
                        <span class="text-gray-400">Whatever you collect,<br>we have it.</span>
                    </h2>
                    <button class="bg-gray-100 hover:bg-gray-200 text-black px-6 py-2 rounded-full text-sm font-medium transition-colors flex items-center gap-2 mx-auto mb-16 mt-8">
                        View all categories
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                            <path d="M5 12h14M12 5l7 7-7 7"/>
                        </svg>
                    </button>

                    <div class="grid grid-cols-2 md:grid-cols-4 gap-px bg-gray-200 border border-gray-200 rounded-2xl overflow-hidden">
                        {#each [
                            {name: 'Gold Coins', icon: '🪙'},
                            {name: 'Silver Coins', icon: '🪙'},
                            {name: 'Gold Bars', icon: '▬'},
                            {name: 'Silver Bars', icon: '▬'},
                            {name: 'Rare Coins', icon: '⭐'},
                            {name: 'Graded Coins', icon: '📜'},
                            {name: 'Platinum', icon: '◆'},
                            {name: 'Palladium', icon: '◆'}
                        ] as category}
                        <div class="bg-[#F9FAFB] p-12 flex flex-col items-center justify-center hover:bg-white transition-all duration-300 group">
                            <div class="text-4xl mb-3 group-hover:scale-110 transition-transform">{category.icon}</div>
                            <span class="font-semibold text-sm text-gray-700">{category.name}</span>
                        </div>
                        {/each}
                    </div>
                </div>

                <!-- Blog Section -->
                <div class="mb-12">
                    <h2 class="text-4xl font-bold text-gray-900 mb-12">Learn about precious metals investing.</h2>
                    <div class="grid md:grid-cols-2 gap-8">
                        <!-- Post 1 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gradient-to-br from-yellow-100 to-yellow-200 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden flex items-center justify-center">
                                <div class="flex gap-2">
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-yellow-400 to-yellow-600 shadow-xl"></div>
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-yellow-400 to-yellow-600 shadow-xl"></div>
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-yellow-400 to-yellow-600 shadow-xl"></div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Buying Guide</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-[var(--color-primary-dark)] transition-colors">Top 5 Gold Coins Every Collector Should Own</h3>
                        </div>
                        <!-- Post 2 -->
                        <div class="group cursor-pointer">
                            <div class="bg-gradient-to-br from-gray-100 to-gray-200 rounded-3xl aspect-[16/9] mb-6 relative overflow-hidden flex items-center justify-center">
                                <div class="flex gap-2">
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-gray-300 to-gray-400 shadow-xl"></div>
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-gray-300 to-gray-400 shadow-xl"></div>
                                    <div class="w-16 h-16 rounded-full bg-gradient-to-br from-gray-300 to-gray-400 shadow-xl"></div>
                                </div>
                            </div>
                            <div class="text-xs font-bold text-gray-500 uppercase tracking-wider mb-2">Market Insights</div>
                            <h3 class="text-2xl font-bold text-gray-900 group-hover:text-[var(--color-primary-dark)] transition-colors">Understanding Spot Prices: A Complete Guide</h3>
                        </div>
                    </div>
                </div>


    </main>

    <Footer />
</div>

