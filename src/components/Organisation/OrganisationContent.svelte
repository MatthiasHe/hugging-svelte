<script>
	import FaMicroscope from 'svelte-icons/fa/FaMicroscope.svelte'
	import FaWarehouse from 'svelte-icons/fa/FaWarehouse.svelte'
	import FaCube from 'svelte-icons/fa/FaCube.svelte'
	import OrganisationModel from './OrganisationModel.svelte'
</script>

<div class="flex py-2 px-4 sm:py-12 sm:px-32">
	<div class="w-1/4">
		<div class="mb-8">
			<div class="font-bold mb-3">
				<span class="w-3 inline-block mr-1"><FaMicroscope/></span>
				Research interests
			</div>
			<p class="mt-2">Solving NLP, one commit at a time</p>
		</div>

		<div>
			<div class="font-bold mb-3">
				<span class="w-3 inline-block mr-1"><FaWarehouse/></span>
				Team members
			</div>

				<div class="grid grid-cols-5 gap-2 pr-12">
				{#each Array(10) as avatar}
					<img
						class="overflow-hidden inline-block rounded-full cursor-pointer hover:shadow-lg"
						alt="avatar"
						src="https://picsum.photos/70"
					>
				{/each}
			</div>
		</div>
	</div>

	<div class="w-3/4">
		<div class="font-bold mb-3">
			<span class="w-3 inline-block mr-1"><FaCube /></span>
			Models
		</div>

		<div class="grid grid-cols-3 gap-10">
			{#each Array(8) as model}
				<OrganisationModel />
			{/each}
		</div>

	</div>
</div>


<style>
</style>
