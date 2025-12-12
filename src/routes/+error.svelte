<script lang="ts">
	import { page } from "$app/state";
</script>

<div class="min-h-screen bg-gradient-to-b from-gray-950 via-gray-900 to-black text-white flex items-center justify-center px-6">
	<div class="max-w-2xl text-center">
		<h1 class="font-serif text-6xl md:text-8xl mb-6">Error {page.status}</h1>
		<p class="text-xl text-gray-300 mb-12">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-flex items-center justify-center px-8 py-4 bg-primary-600 hover:bg-primary-700 rounded-full text-base font-medium text-white transition-colors duration-300">
			Go back home
		</a>
	</div>
</div>
