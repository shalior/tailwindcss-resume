<script lang="ts">
	export let title = 'SkiLL';
	export let rate: 1 | 2 | 3 | 4 | 5 = 5;
</script>

<div class="">
	<h6 class="font-bold">{title}</h6>

	<div class="stars inline-flex space-x-1">
		{#each [1, 2, 3, 4, 5] as _, i}
			<i class="material-icons mt-1 {_ > rate ? 'text-gray-400' : 'text-amber-500'}">star</i>
		{/each}
	</div>
</div>
