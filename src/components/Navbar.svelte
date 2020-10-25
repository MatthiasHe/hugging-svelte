<script>
	import MdClose from 'svelte-icons/md/MdClose.svelte'
	import MdMenu from 'svelte-icons/md/MdMenu.svelte'

	let hidden = false;

	function navActionClick() {
		hidden = !hidden;
	}
</script>

<header class="sm:flex sm:justify-between sm:items-center sm:px-4 sm:py-3 border-b-2 lg:py-6 lg:px-32">
	<div class="flex items-center justify-between px-4 py-3 sm:p-0">
		<span class="font-bold text-xl tracking-tight mr-4">Hugging Face</span>

		<input
			placeholder="Search models, datasets, users..."
			class="border border-gray-300 placeholder-gray-500 text-gray-900 rounded-full pl-4 pr-16 py-1 appearance-none"
		>

		<div class="sm:hidden">
			<button on:click={navActionClick} type="button" class="block border-none focus:outline-none w-8">
				{#if hidden}
					<MdMenu />
				{:else}
					<MdClose />
				{/if}
			</button>
		</div>
	</div>

	<nav class="px-2 pt-2 pb-4 sm:flex sm:p-0">
		<a class="block mt-4 lg:inline-block lg:mt-0 hover:text-purple-800 mr-4 cursor-pointer">Models</a>
		<a class="block mt-4 lg:inline-block lg:mt-0 hover:text-purple-800 mr-4 cursor-pointer">Pricing</a>
		<a class="block mt-4 lg:inline-block lg:mt-0 underline hover:text-purple-800 cursor-pointer">Account</a>
	</nav>
</header>

<style>
</style>
