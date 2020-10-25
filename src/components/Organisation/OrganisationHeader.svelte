<script>
	const href = 'https://huggingface.com';
	const src = 'https://aeiljuispo.cloudimg.io/v7/https://s3.amazonaws.com/moonup/production/uploads/1583856921041-5dd96eb166059660ed1ee413.png?w=200&h=200&f=face';
</script>

<div class="py-2 px-4 flex flex-col items-center bg-gray-100 sm:py-12 sm:px-32 sm:flex-row">
	<img class="h-24 rounded" {src}/>

	<div class="pl-8 text-center sm:text-left">
		<h1 class="font-bold text-3xl">Hugging Face</h1>
		<div class="flex items-center">
			<span class="bold rounded bg-purple-200 text-purple-800 p-1 px-2">Company</span>
			<span class="dot rounded-full bg-gray-400 mx-2"></span>
			<a {href}>{href}</a>
		</div>
	</div>
</div>

<style>
	.dot {
		width: 0.35rem;
		height: 0.35rem;
	}
</style>
