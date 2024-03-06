<script>
	export let title = '';
	export let description = '';
	export let image = '';
</script>

<article>
	<h3>{title}</h3>
	<details>
		<summary>
			<em>Click to see more</em>
		</summary>
		<div class="article-content">
			<p>
				{description}
			</p>
			<img src={image} alt="" />
		</div>
	</details>
</article>
