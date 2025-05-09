<script>
	export let title = "";
	export let content = "";
	export let image = "";
	export let funFact = "This is a fun card!";
</script>

<div class="card">
	{#if image}
		<img src={image} alt={title} class="card-image" />
	{/if}
	<div class="card-content">
		<h2 class="card-title">{title}</h2>
		<p class="card-text">{content}</p>
		<p class="card-fun">{funFact}</p>
	</div>
</div>

<style>
	.card {
		border: 1px solid #ddd;
		border-radius: 8px;
		overflow: hidden;
		box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
		max-width: 300px;
	}
	.card-image {
		width: 100%;
		height: auto;
	}
	.card-content {
		padding: 16px;
	}
	.card-title {
		margin: 0 0 8px;
		font-size: 1.25rem;
	}
	.card-text {
		margin: 0;
		color: #555;
	}
	.card-fun {
		margin-top: 8px;
		font-style: italic;
		color: #888;
	}
</style>
