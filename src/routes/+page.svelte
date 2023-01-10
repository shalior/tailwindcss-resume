<script lang="ts">
	import Skill from '$lib/components/Skill.svelte';
	import '../app.css';
	import Experience from '$lib/components/Experience.svelte';
	import Github from '$lib/icons/Github.svelte';
</script>

<svelte:head>
	<!-- Material Icons -->
	<link rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons" />
	<title>TailwindCSS Resume</title>
</svelte:head>

<div class="p-6 font-sans text-gray-800 font-calibri" style="width: 210mm; height: auto">
	<div class="grid grid-cols-7">
		<main class="col-span-5 pr-4">
			<header>
				<h1 class="text-5xl font-bold">Jhon Doe</h1>
				<p class="text-gray-700 mt-2">Full stack developer</p>
			</header>

			<section class="mt-6">
				<h1 class="text-3xl inline-flex items-center">
					<i class="material-icons !text-3xl text-stone-700 mr-4">person</i>
					About me
				</h1>

				<p class="text-gray-700 mt-2 prose text-justify">
					Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iste doloribus veritatis
					blanditiis excepturi omnis necessitatibus hic. Fugit reprehenderit a quam distinctio ex,
					ratione ducimus iusto quos ad, non, architecto voluptatem!
				</p>
			</section>

			<hr class="my-6 shadow-sm" />

			<section>
				<h1 class="text-3xl inline-flex items-center">
					<i class="material-icons !text-3xl text-stone-700 mr-4">history</i>
					Experiences
				</h1>

				<Experience
					role="Full-Stack developer"
					location="Remote"
					dateRange="Apr 2293 - Present"
					company="Example.company"
				>
					<p class="prose text-justify text-sm text-gray-600">
						Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iste doloribus veritatis
						blanditiis excepturi omnis necessitatibus hic. Fugit reprehenderit a quam distinctio ex,
						ratione ducimus iusto quos ad, non, architecto voluptatem!
					</p>
				</Experience>

				<Experience
					role="Full-Stack developer"
					location="Remote"
					dateRange="Apr 2293 - Present"
					company="Example.company"
				>
					<p class="prose text-justify text-sm text-gray-600">
						Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iste doloribus veritatis
						blanditiis excepturi omnis necessitatibus hic. Fugit reprehenderit a quam distinctio ex,
						ratione ducimus iusto quos ad, non, architecto voluptatem!
					</p>
				</Experience>

				<Experience
					role="Full-Stack developer"
					location="Remote"
					dateRange="Apr 2293 - Present"
					company="Example.company"
				>
					<p class="prose text-justify text-sm text-gray-600">
						Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iste doloribus veritatis
						blanditiis excepturi omnis necessitatibus hic. Fugit reprehenderit a quam distinctio ex,
						ratione ducimus iusto quos ad, non, architecto voluptatem!
					</p>
				</Experience>

				<Experience role="Freelancer" location="Remote" dateRange="Jan 1444 - Oct 1245">
					<p class="prose text-justify text-sm text-gray-600">
						Lorem ipsum dolor sit amet consectetur, adipisicing elit. Iste doloribus veritatis
						blanditiis excepturi omnis necessitatibus hic. Fugit reprehenderit a quam distinctio ex,
						ratione ducimus iusto quos ad, non, architecto voluptatem!
					</p>
				</Experience>
			</section>
		</main>

		<aside class="col-span-2">
			<section>
				<h4 class="text-xl font-semibold mb-3">Personal info</h4>

				<ul class="space-y-2 text-sm pl-2">
					<li class="text-gray-500">
						Phone: <span class="text-gray-700 font-bold">00000000000</span>
					</li>
					<li class="text-gray-500">
						Email: <span class="text-gray-700 font-bold">ali_shalior@proton.me</span>
					</li>
					<li class="text-gray-500">
						Location: <span class="text-gray-700 font-bold">Earth</span>
					</li>
					<li class="text-gray-500">
						DoB: <span class="text-gray-700 font-bold">Apr 1880</span>
					</li>
					<li class="text-gray-500">
						Education: <span class="text-gray-700 font-bold">Bachelor CS</span>
					</li>
				</ul>
			</section>

			<hr class=" my-4 shadow-sm" />

			<section>
				<h4 class="text-xl font-semibold mb-3">Skills</h4>

				<div class="skills space-y-4 pl-2">
					<Skill title="JavaScript & TypeScript" rate={5} />
					<Skill title="PHP" rate={5} />
					<Skill title="CI/CD" rate={5} />
					<Skill title="Git and GitHub" rate={5} />
					<Skill title="Test driven development" rate={5} />
					<Skill title="Svelte Kit" rate={1} />
					<Skill title="TailwindCSS" rate={5} />
					<Skill title="Docker" rate={4} />
					<Skill title="NoSQL" rate={3} />
				</div>
			</section>

			<hr class=" my-4 shadow-sm" />

			<section>
				<h4 class="text-xl font-semibold mb-3">Links</h4>

				<ul class="links space-y-2 pl-2">
					<li class="inline-flex items-center gap-2 flex-wrap font-bold">
						<Github />
						GitHub
						<a class="text-gray-600" href="https://github.com/shalior">https://github.com/shalior</a
						>
					</li>
				</ul>
			</section>
		</aside>
	</div>
</div>

<style>
	.font-calibri {
		font-family: 'Calibri', sans-serif;
	}
</style>
