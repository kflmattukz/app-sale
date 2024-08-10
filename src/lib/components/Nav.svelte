<script>
	const links = [
		{
			href: '/',
			name: 'home'
		},
		{
			href: '/blogs',
			name: 'blogs'
		},
		{
			href: '/about',
			name: 'about'
		}
	];
</script>

<nav class="bg-gray-200 px-10 py-5">
	<div class="container mx-auto flex w-2/3 items-center justify-between">
		<a class="logo text-2xl font-bold capitalize" href="/">App-Sale</a>
		<div class="links space-x-10">
			{#each links as link}
				<a href={link.href}>{link.name}</a>
			{/each}
		</div>
	</div>
</nav>
