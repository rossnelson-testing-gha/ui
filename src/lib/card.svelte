<script>
	export let title = "";
	export let content = "";
	export let image = "";
</script>

<div class="card">
	{#if image}
		<img src={image} alt={title} class="card-image" />
	{/if}
	<div class="card-content">
		<h2 class="card-title">{title}</h2>
		<p class="card-text">{content}</p>
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
</style>
