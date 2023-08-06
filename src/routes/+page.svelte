<script>
    import { userData } from "$lib/firebase";
</script>
  
<svelte:head>
<title>Linktree Clone</title>
<meta name="description" content="Linktree Clone" />
</svelte:head>
  
<main class="flex w-full min-h-screen">

<div class="hero bg-base-200">
	<div class="hero-content text-center">
	<div class="w-full">
		<h1 class="h1 text-6xl text-center">
			<span class="bg-gradient-to-br from-green-500 to-yellow-300 bg-clip-text text-transparent box-decoration-clone">Linktree Clone🌴</span>
		</h1>
		<p class="py-6 text-2xl">One link for all your links 🔗</p>
		{#if $userData?.username}
		<a href="/{$userData.username}/edit" class="btn btn-primary">Edit Profile</a>
		{:else}
		<a href="/login" class="btn btn-primary">Get Started</a>
		<a href="/kyle1" class="btn btn-secondary">Example Profile</a>
		{/if}
		<p class="py-6">Built from scratch using the 🔥Fireship <a class="link" href="https://fireship.io/courses/sveltekit">SvelteKit Course</a></p>
	</div>
	</div>
</div>

</main>
