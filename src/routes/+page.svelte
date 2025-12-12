<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:head>
	<title>Ballpoint - Creative-Driven Performance Marketing for DTC Brands</title>
	<meta name="description" content="We transform early-stage brands into household names through creative-driven performance marketing. Proven frameworks for TikTok, Meta, and YouTube ads that drive profitable growth." />
	<meta property="og:title" content="Ballpoint - Creative-Driven Performance Marketing" />
	<meta property="og:description" content="Scientific growth frameworks meet breakthrough creative. We help DTC founders achieve profitable customer acquisition." />
	<meta property="og:type" content="website" />
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content="Ballpoint - Creative-Driven Performance Marketing" />
	<meta name="twitter:description" content="We transform early-stage brands into household names through creative-driven performance marketing." />
</svelte:head>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-200 selection:text-primary-900">
	<!-- Navigation / Header -->
	<header class="fixed top-0 left-0 right-0 z-50 bg-white/80 backdrop-blur-md border-b border-gray-100">
		<div class="px-6 md:px-12 lg:px-24 py-4 flex items-center justify-between">
			<a href="/" class="flex items-center gap-2">
				<svg class="w-8 h-8 text-gray-900" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386ZM14.261 4.12767L13.7751 4.96887L18.9438 13.9213H19.9139L14.261 4.12767ZM13.1286 6.08808L12.6467 6.9225L16.6749 13.9006L16.6634 13.9213H17.6511L13.1286 6.08808ZM11.9999 8.04225L8.60411 13.9213H15.3899L11.9999 8.04225ZM6.99833 3.30006C7.33866 3.10343 7.7248 2.99993 8.11786 3L2.30033 13.0776C2.10357 12.7371 2 12.3508 2 11.9575C2 11.5643 2.10357 11.178 2.30033 10.8375L6.17916 4.12006C6.37543 3.77951 6.65798 3.49669 6.99833 3.30006ZM9.08869 3H10.3816L3.43223 15.0384L2.785 13.9184L9.08869 3ZM11.3509 3H12.6424L4.56262 16.9963L3.91691 15.8777L11.3509 3ZM21.7064 13.0598C21.8988 12.7254 22 12.3463 22 11.9605C22 11.5746 21.8988 11.1956 21.7064 10.8611L17.8039 4.10233C17.6108 3.7681 17.3331 3.49057 16.9987 3.2976C16.6644 3.10463 16.2852 3.00302 15.8992 3.00296H15.8741L21.6931 13.082L21.7064 13.0598ZM17.7995 19.7994H6.17916C6.37472 20.1412 6.65692 20.4253 6.99728 20.6232C7.33763 20.8212 7.72414 20.9258 8.11786 20.9269H15.8829C16.2737 20.9261 16.6572 20.8212 16.994 20.6231C17.3309 20.4249 17.6089 20.1406 17.7995 19.7994Z"
						fill="currentColor"
					/>
				</svg>
				<span class="font-bold text-xl">Ballpoint</span>
			</a>
			<nav class="hidden md:flex items-center gap-8 text-sm font-medium">
				<a href="#work" class="hover:text-primary-600 transition-colors">Work</a>
				<a href="#approach" class="hover:text-primary-600 transition-colors">Approach</a>
				<a href="#insights" class="hover:text-primary-600 transition-colors">Insights</a>
				<a href="#contact" class="inline-flex items-center justify-center px-4 py-2 bg-gray-900 text-white rounded-full hover:bg-gray-800 transition-colors">
					Get in touch
				</a>
			</nav>
		</div>
	</header>

	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-gradient-to-b from-gray-950 via-gray-900 to-white text-white px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-center">
		<div class="max-w-5xl">
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight mb-8">
				We transform early-stage brands into household names through creative-driven performance marketing.
			</h1>
			<p class="text-xl md:text-2xl text-gray-300 max-w-3xl mb-12">
				Scientific growth frameworks meet breakthrough creative. We help DTC founders achieve profitable customer acquisition through TikTok, Meta, and YouTube.
			</p>
		</div>

		<div class="mt-12">
			<a href="#work" class="inline-flex items-center justify-center px-6 py-3 border border-white/30 rounded-full text-sm font-medium hover:bg-white hover:text-gray-900 transition-colors duration-300 backdrop-blur-sm">
				See our work
			</a>
		</div>
	</section>

	<!-- Trusted Clients -->
	<section class="bg-white px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12">Trusted by ambitious DTC brands on their journey to scale</p>
		
		<div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-4 gap-6 md:gap-8">
			<!-- Client logos -->
			{#each ['Thriva', 'Mother Root', 'Tilly Sveaas', 'Citizens of Soil', 'Chatsie', 'Glaize', 'Tuza', 'Sipgood'] as client}
				<div class="h-20 bg-gray-50 rounded-lg flex items-center justify-center grayscale opacity-60 hover:opacity-100 hover:grayscale-0 transition-all duration-300 border border-gray-100">
					<span class="font-semibold text-gray-800 text-sm md:text-base">{client}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Work Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="work">
        <div class="flex flex-col md:flex-row justify-between items-end mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900">Brands we've helped scale from zero to hero</h2>
            <a href="/work" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                See all case studies <span class="ml-2">→</span>
            </a>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Project 1: Thriva -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Thriva</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Scaled from zero to 100,000 customers through creative-first performance marketing. Built a sustainable acquisition engine across Meta and TikTok that drove profitable growth.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Performance Marketing</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Creative Strategy</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Scale</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-900 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-young-founder-working-confidently-at-des-1765570743637-4.webp" alt="Thriva campaign" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 2: Mother Root -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Mother Root</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Launched TikTok-first creative strategy that achieved 3x ROAS in first 90 days. Developed breakthrough ad frameworks that resonated with health-conscious millennials.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">TikTok Ads</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Creative Testing</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-person-filming-creative-content-for-soci-1765570738687-2.webp" alt="Mother Root campaign" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 3: Tilly Sveaas -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Tilly Sveaas</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Built a full-funnel Meta advertising strategy that drove 250% revenue growth. Optimized creative production workflow to test 50+ ad variations monthly while maintaining brand aesthetics.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Meta Ads</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">CRO</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Creative Production</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-creative-team-brainstorming-marketing-ca-1765570733147-0.webp" alt="Tilly Sveaas campaign" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Project 4: Citizens of Soil -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-4 space-y-6">
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Citizens of Soil</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Developed YouTube advertising strategy that reduced CAC by 40% while scaling spend 5x. Created educational content framework that built trust and drove conversions for premium product.
                    </p>
                    <div class="flex flex-wrap gap-2 pt-2">
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">YouTube Ads</span>
                        <span class="px-3 py-1 border border-gray-200 rounded-full text-xs font-medium text-gray-600">Content Strategy</span>
                    </div>
                </div>
                <div class="lg:col-span-8">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="/generated/image-excited-startup-team-celebrating-success-1765570741244-3.webp" alt="Citizens of Soil campaign" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>
        </div>
        
        <div class="mt-12 md:hidden">
            <a href="/work" class="flex items-center text-gray-500 hover:text-gray-900 transition-colors">
                See all case studies <span class="ml-2">→</span>
            </a>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24" id="approach">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-16 max-w-3xl">Our approach: Scientific growth frameworks meet breakthrough creative</h2>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Creative Strategy -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Creative Strategy</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We analyze your market, audience, and competitors to develop data-driven creative hypotheses. Every campaign starts with a clear strategy rooted in growth fundamentals.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-entrepreneur-founder-reviewing-analytics-1765570736342-1.webp" alt="Strategy" class="h-full w-full object-cover rounded-lg" />
                </div>
            </div>

            <!-- Performance Testing -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Performance Testing</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    We rapidly produce and test creative variations across TikTok, Meta, and YouTube. Fast iteration cycles help us identify winning formulas and kill losers quickly.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-person-filming-creative-content-for-soci-1765570738687-2.webp" alt="Testing" class="h-full w-full object-cover rounded-lg" />
                </div>
            </div>

            <!-- Scale & Optimize -->
            <div class="bg-white p-8 rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300 flex flex-col h-full min-h-[400px]">
                <h3 class="text-xl font-semibold mb-4">Scale & Optimize</h3>
                <p class="text-gray-600 text-sm leading-relaxed mb-auto">
                    Once we find what works, we scale aggressively while continuously optimizing. We build sustainable acquisition engines that deliver profitable growth month after month.
                </p>
                <div class="mt-8 flex justify-center h-48 items-end">
                    <img src="/generated/image-excited-startup-team-celebrating-success-1765570741244-3.webp" alt="Scale" class="h-full w-full object-cover rounded-lg" />
                </div>
            </div>
        </div>
    </section>

    <!-- Insights Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="insights">
        <div class="flex flex-col md:flex-row justify-between items-end mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900">Growth insights from the frontlines</h2>
            <a href="/insights" class="hidden md:inline-flex items-center text-gray-500 hover:text-gray-900 transition-colors mt-4 md:mt-0">
                Read all <span class="ml-2">→</span>
            </a>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Blog Post 1 -->
            <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-primary-600 to-primary-800 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white font-bold text-3xl text-center p-8">
                        <span>The TikTok Ad Framework That Scales</span>
                     </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">How we built a repeatable system for testing 50+ TikTok ads per month</h3>
            </div>

             <!-- Blog Post 2 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                    <img src="/generated/image-creative-team-reviewing-tiktok-ads-on-mo-1765570746089-5.webp" alt="Creative testing" class="w-full h-full object-cover opacity-70" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Why Creative-First Beats Targeting Every Time</h3>
            </div>

             <!-- Blog Post 3 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-gray-800 to-gray-950 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white text-center p-8 flex-col">
                        <span class="text-4xl font-bold mb-2">3X</span>
                        <span class="text-lg">ROAS in 90 Days</span>
                     </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">The exact framework we use to scale DTC brands from £0 to £1M</h3>
            </div>

             <!-- Blog Post 4 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-100 rounded-lg overflow-hidden mb-4 relative">
                    <img src="/generated/image-entrepreneur-founder-reviewing-analytics-1765570736342-1.webp" alt="Analytics" class="w-full h-full object-cover" />
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">From Thriva to 100,000 Customers: Lessons in Scaling</h3>
            </div>

             <!-- Blog Post 5 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gradient-to-br from-primary-500 to-primary-700 rounded-lg overflow-hidden mb-4 relative flex items-center justify-center">
                    <div class="text-white text-center p-8">
                        <div class="text-5xl font-bold mb-4">📱</div>
                        <div class="text-xl font-semibold">UGC vs Studio</div>
                    </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">When to use UGC creators vs professional production for your ads</h3>
            </div>

             <!-- Blog Post 6 -->
             <div class="group cursor-pointer">
                <div class="aspect-square bg-gray-900 rounded-lg overflow-hidden mb-4 relative">
                     <div class="absolute inset-0 flex items-center justify-center text-white text-center p-8">
                        <span class="text-2xl font-serif leading-tight">Probabilistic thinking beats deterministic planning</span>
                     </div>
                </div>
                <h3 class="text-sm font-medium text-gray-900 group-hover:underline">Why growth is a science, not an art: Our philosophy on performance marketing</h3>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12">
        <div class="bg-gradient-to-br from-gray-900 to-gray-950 rounded-2xl p-8 md:p-16 lg:p-20 text-white">
            <h3 class="font-serif text-2xl md:text-3xl mb-4">Get growth insights delivered monthly</h3>
            <p class="text-gray-300 mb-8 max-w-md">Real frameworks, case studies, and creative strategies from the trenches. No fluff, just what's working right now.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-lg">
                <input type="email" placeholder="founder@yourcompany.com" class="flex-1 bg-white/10 border border-white/20 rounded-lg px-4 py-3 text-sm placeholder:text-gray-400 focus:ring-1 focus:ring-primary-500 outline-none text-white" />
                <button type="submit" class="bg-primary-600 hover:bg-primary-700 transition-colors text-white px-6 py-3 rounded-lg text-sm font-medium">
                    Subscribe
                </button>
            </form>
            <p class="text-[10px] text-gray-400 mt-4">We respect your inbox. Unsubscribe anytime. By signing up, you agree to receive communications from Ballpoint.</p>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="relative bg-gradient-to-b from-gray-900 via-gray-950 to-black pt-32 pb-48 px-6 md:px-12 lg:px-24 overflow-hidden" id="contact">
        <div class="max-w-5xl relative z-10">
            <h2 class="font-serif text-4xl md:text-6xl lg:text-7xl text-white leading-tight mb-8">
                Ready to scale your brand? <br />
                <span class="text-gray-400">Let's build your growth engine together.</span>
            </h2>
            <p class="text-xl text-gray-300 max-w-2xl mb-12">
                We work with ambitious founders who are ready to invest in creative-driven performance marketing. If you're doing at least £10k/month in revenue and ready to scale, let's talk.
            </p>
            
            <div class="mt-16 flex flex-col sm:flex-row gap-4">
                 <a href="mailto:hello@ballpoint.agency" class="inline-flex items-center justify-center px-8 py-4 bg-primary-600 hover:bg-primary-700 rounded-full text-base font-medium text-white transition-colors duration-300">
                    Get in touch
                </a>
                <a href="#work" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 rounded-full text-base font-medium text-white hover:bg-white hover:text-gray-900 transition-colors duration-300">
                    View case studies
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-gray-300 px-6 md:px-12 lg:px-24 pt-24 pb-12 relative overflow-hidden">
        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-24">
                <div class="col-span-1 md:col-span-2">
                    <a href="/" class="flex items-center gap-2 mb-8">
                        <svg class="w-10 h-10 text-white" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                fill-rule="evenodd"
                                clip-rule="evenodd"
                                d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386ZM14.261 4.12767L13.7751 4.96887L18.9438 13.9213H19.9139L14.261 4.12767ZM13.1286 6.08808L12.6467 6.9225L16.6749 13.9006L16.6634 13.9213H17.6511L13.1286 6.08808ZM11.9999 8.04225L8.60411 13.9213H15.3899L11.9999 8.04225ZM6.99833 3.30006C7.33866 3.10343 7.7248 2.99993 8.11786 3L2.30033 13.0776C2.10357 12.7371 2 12.3508 2 11.9575C2 11.5643 2.10357 11.178 2.30033 10.8375L6.17916 4.12006C6.37543 3.77951 6.65798 3.49669 6.99833 3.30006ZM9.08869 3H10.3816L3.43223 15.0384L2.785 13.9184L9.08869 3ZM11.3509 3H12.6424L4.56262 16.9963L3.91691 15.8777L11.3509 3ZM21.7064 13.0598C21.8988 12.7254 22 12.3463 22 11.9605C22 11.5746 21.8988 11.1956 21.7064 10.8611L17.8039 4.10233C17.6108 3.7681 17.3331 3.49057 16.9987 3.2976C16.6644 3.10463 16.2852 3.00302 15.8992 3.00296H15.8741L21.6931 13.082L21.7064 13.0598ZM17.7995 19.7994H6.17916C6.37472 20.1412 6.65692 20.4253 6.99728 20.6232C7.33763 20.8212 7.72414 20.9258 8.11786 20.9269H15.8829C16.2737 20.9261 16.6572 20.8212 16.994 20.6231C17.3309 20.4249 17.6089 20.1406 17.7995 19.7994Z"
                                fill="currentColor"
                            />
                        </svg>
                        <span class="font-bold text-2xl text-white">Ballpoint</span>
                    </a>
                    <p class="text-gray-400 max-w-md mb-8">
                        Creative-driven performance marketing for ambitious DTC brands. We help early-stage founders build profitable acquisition engines.
                    </p>
                    <a href="mailto:hello@ballpoint.agency" class="text-xl font-medium text-white hover:text-primary-400 transition-colors inline-flex items-center">
                        hello@ballpoint.agency <span class="ml-2">→</span>
                    </a>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-medium text-white">London Office</h4>
                    <div class="text-sm space-y-2">
                        <p>Clerkenwell/Farringdon</p>
                        <p>London, UK</p>
                        <p class="mt-4 text-gray-500">Four days per week in office</p>
                        <p class="text-gray-500">Flexible Mondays</p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center border-t border-gray-800 pt-8">
                <div class="flex gap-8 text-sm mb-4 md:mb-0">
                    <a href="#work" class="hover:text-white transition-colors">Work</a>
                    <a href="#approach" class="hover:text-white transition-colors">Approach</a>
                    <a href="#insights" class="hover:text-white transition-colors">Insights</a>
                    <a href="/careers" class="hover:text-white transition-colors">Careers</a>
                </div>
                
                <div class="flex gap-6 text-sm">
                    <a href="https://linkedin.com/company/ballpoint" class="hover:text-white transition-colors">LinkedIn</a>
                    <a href="https://twitter.com/ballpoint" class="hover:text-white transition-colors">Twitter</a>
                    <a href="https://instagram.com/ballpoint" class="hover:text-white transition-colors">Instagram</a>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between text-xs text-gray-500 mt-12">
                <p>© 2025 Ballpoint. All rights reserved.</p>
                <p>Privacy Policy</p>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

