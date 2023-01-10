<script lang="ts">
	export let role = 'Role';
	export let company = '';
	export let location = '';
	export let dateRange = '';
</script>

<div class="pl-2 mt-4">
	<h1 class="role text-xl text-gray-800 font-bold inline-flex items-center">
		<i class="material-icons !text-sm text-gray-500 mr-2">circle</i>
		{role}
	</h1>

	<div class="meta text-gray-700 mt-1 flex justify-between text-xs">
		{#if company}
			<p class="inline-flex items-center">
				<i class="material-icons !text-base text-gray-500 mr-2">apartment</i>
				<span>
					{company}
				</span>
			</p>
		{/if}

		{#if location}
			<p class="inline-flex items-center">
				<i class="material-icons !text-base text-gray-500 mr-2">location_on</i>
				<span>
					{location}
				</span>
			</p>
		{/if}

		{#if dateRange}
			<p class="inline-flex items-center">
				<i class="material-icons !text-base text-gray-500 mr-2">date_range</i>
				<span>
					{dateRange}
				</span>
			</p>
		{/if}
	</div>

	<div class="description text-gray-700 mt-2">
		<slot />
	</div>
</div>
