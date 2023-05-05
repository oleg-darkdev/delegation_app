<script>
	let open = false;
</script>

<header class=" flex  w-full justify-center">
	<div
		x-data={open}
		class="mx-auto flex max-w-screen-xl flex-col p-5 md:flex-row md:items-center md:justify-between md:px-6 lg:px-8"
	>
		<div class="flex flex-row items-center justify-between lg:justify-start">
			<a
				href="./index.html"
				class="tracking-relaxed transform text-lg font-bold tracking-tighter text-blue-600 transition duration-500 ease-in-out lg:pr-8"
			>
				wickedblocks
			</a>
			<button
				class="focus:shadow-outline rounded-lg focus:outline-none md:hidden"
				on:click={() => (open = !open)}
			>
				<svg fill="currentColor" viewBox="0 0 20 20" class="h-8 w-8">
					<path
						x-show="!open"
						fill-rule="evenodd"
						d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
						clip-rule="evenodd"
					/>
					<path
						x-show="open"
						fill-rule="evenodd"
						d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
						clip-rule="evenodd"
						style="display: none"
					/>
				</svg>
			</button>
		</div>
		<nav
			:class="'flex': {open}, 'hidden': {!open}"
			class="hidden flex-grow flex-col md:flex md:flex-row md:justify-end"
		>
			<ul class="list-none space-y-2 lg:inline-flex lg:items-center lg:space-y-0">
				<li>
					<a
						href="#theory"
						class="border-b-2 border-transparent px-2 py-6 text-sm leading-[22px] text-gray-500 hover:border-blue-600 hover:text-blue-500 md:px-3 lg:px-6"
					>
						<span class="hidden lg:inline">Teoria stopniej delegowania </span>
					</a>
				</li>
				<li>
					<a
						href="#"
						class="border-b-2 border-transparent px-2 py-6 text-sm leading-[22px] text-gray-500 hover:border-blue-600 hover:text-blue-500 md:px-3 lg:px-6"
					>
						Warsztaty
					</a>
				</li>
				<li>
					<a
						href="/app"
						class="border-b-2 border-transparent px-2 py-6 text-sm leading-[22px] text-gray-500 hover:border-blue-600 hover:text-blue-500 md:px-3 lg:px-6"
					>
						Web Aplikacja
					</a>
				</li>

				<li>
					<a
						href="#"
						class="border-b-2 border-transparent px-2 py-6 text-sm leading-[22px] text-gray-500 hover:border-blue-600 hover:text-blue-500 md:px-3 lg:px-6"
					>
						FAQ
					</a>
				</li>
				<li>
					<a
						href="#"
						class="border-b-2 border-transparent px-2 py-6 text-sm leading-[22px] text-gray-500 hover:border-blue-600 hover:text-blue-500 md:px-3 lg:px-6"
					>
						Contact <span class="hidden lg:inline" />
					</a>
				</li>
			</ul>
		</nav>
	</div>
</header>

<a name="faq" />
<a name="contact" />
<a name="workshops" />

<main class="">
	<section>
		<div class="mx-auto max-w-7xl px-4 py-12 sm:px-6 md:px-12 lg:px-24 ">
			<div class=" flex w-full flex-col text-center">
				<!-- <div
				class="mx-auto mb-5 inline-flex h-20 w-20 flex-shrink-0 items-center justify-center rounded-full bg-gray-50 text-blue-600"
			>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					class="icon icon-tabler icon-tabler-aperture h-10 w-10"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					fill="none"
					stroke-linecap="round"
					stroke-linejoin="round"
				>
					<path stroke="none" d="M0 0h24v24H0z" fill="none" />
					<circle cx="12" cy="12" r="9" />
					<line x1="3.6" y1="15" x2="14.15" y2="15" />
					<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(72 12 12)" />
					<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(144 12 12)" />
					<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(216 12 12)" />
					<line x1="3.6" y1="15" x2="14.15" y2="15" transform="rotate(288 12 12)" />
				</svg>
			</div> -->
				<h1
					class="max-w-5xl text-2xl font-bold leading-none tracking-tighter text-neutral-600 md:text-5xl lg:max-w-7xl lg:text-6xl"
				>
					Long headline to turn <br class="hidden lg:block" />
					your visitors into users
				</h1>

				<p class="mx-auto mt-8 max-w-xl text-center text-base leading-relaxed text-gray-500">
					Free and Premium themes, UI Kit's, templates and landing pages built with Tailwind CSS,
					HTML &amp; Next.js.
				</p>

				<a
					class="mx-auto mt-8 text-sm font-semibold text-blue-600 hover:text-neutral-600"
					title="read more"
				>
					Read more about the offer »
				</a>
			</div>
		</div>
	</section>

	<section class="flex w-full justify-center">
		<div class=" max-w-5xl ">
			<!-- <div class="border-b border-gray-600 pb-4">
		</div> -->
			<!-- <h3 class="text-xl font-semibold leading-6 text-gray-800 text-center">Пример диалога</h3> -->

			<div class="relative mx-auto w-full">
				<div class="mx-auto mt-12 grid max-w-lg gap-8 lg:max-w-none lg:grid-cols-2">
					<div class="mb-12 flex cursor-pointer flex-col overflow-hidden">
						<a href="/blog-post">
							<div class="flex-shrink-0">
								<img
									class="h-48 w-full rounded-lg object-cover"
									src="/assets/images/placeholders/neon-2.jpg"
									alt=""
								/>
							</div>
						</a>

						<div class="flex flex-1 flex-col justify-between">
							<a href="/blog-post" />
							<div class="flex-1">
								<a href="/blog-post">
									<div class="flex space-x-1 pt-6 text-sm text-gray-500">
										<time datetime="2020-03-10"> Mar 10, 2020 </time>
										<span aria-hidden="true"> · </span>
										<span> 4 min read </span>
									</div>
								</a>
								<a href="#" class="mt-2 block space-y-6">
									<h3 class="text-2xl font-semibold leading-none tracking-tighter text-neutral-600">
										Typography on app.
									</h3>
									<p class="text-lg font-normal text-gray-500">
										Filling text so you can see how it looks like with text. Did I said text?
									</p>
									<!-- <div class="mt-6 flex items-center">
								<div>
									<img
										class="inline-block h-9 w-9 rounded-full"
										src="/assets/images/placeholders/avatar-bw-1.jpg"
										alt=""
									/>
								</div>
								<div class="ml-3">
									<p class="text-sm font-medium text-gray-700 group-hover:text-neutral-600">
										Jazz Torp
									</p>
								</div>
							</div> -->
								</a>
							</div>
						</div>
					</div>

					<div class="lg:grid lg:grid-cols-2 ">
						<div class="mb-12 flex cursor-pointer flex-col overflow-hidden">
							<a href="/blog-post">
								<div class="flex-shrink-0">
									<img
										class="h-48 w-full rounded-lg object-cover"
										src="/assets/images/placeholders/neon-5.jpg"
										alt=""
									/>
								</div>
							</a>
							<div class="flex flex-1 flex-col justify-between">
								<a href="/blog-post" />
								<div class="flex-1">
									<a href="/blog-post">
										<div class="flex space-x-1 pt-6 text-sm text-gray-500">
											<time datetime="2020-03-10"> Mar 10, 2020 </time>
											<span aria-hidden="true"> · </span>
											<span> 4 min read </span>
										</div>
									</a>
									<a href="#" class="mt-2 block space-y-6">
										<h3
											class="text-2xl font-semibold leading-none tracking-tighter text-neutral-600"
										>
											Typography on app.
										</h3>
										<p class="text-lg font-normal text-gray-500">
											Filling text so you can see how it looks like with text. Did I said text?
										</p>

										<!-- <div class="mt-6 flex items-center">
									<div>
										<img
											class="inline-block h-9 w-9 rounded-full"
											src="/assets/images/placeholders/avatar-bw-2.jpg"
											alt=""
										/>
									</div>
									<div class="ml-3">
										<p class="text-sm font-medium text-gray-700 group-hover:text-neutral-600">
											Robert Zox
										</p>
									</div>
								</div> -->
									</a>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>

	<section class="flex justify-center">
		<div class="max-w-4xl">
			<div class="relative ">
				<div class="relative flex justify-start">
					<span class="bg-white pr-3 text-lg font-medium text-neutral-600"
						>Ступени делегирования</span
					>
				</div>
			</div>
			<a name="theory" />
			<div class="space-y-8 lg:divide-y lg:divide-gray-100">
				<div class="group pt-8 sm:flex lg:items-end">
					<div class="mb-4 flex-shrink-0 sm:mb-0 sm:mr-4">
						<img
							class="h-32 w-full rounded-md object-cover lg:w-32"
							src="/assets/images/placeholders/neon-1.jpg"
							alt="text"
						/>
					</div>
					<div>
						<span class="text-sm text-gray-500">August 20.20.21</span>
						<p class="mt-3 text-lg font-medium leading-6">
							<a
								href="./blog-post.html"
								class="text-xl text-gray-800 group-hover:text-gray-500 lg:text-2xl"
								>12 Graphic Design Skills You Need To Get Hired (&amp; How to Develop Them)
							</a>
						</p>
						<p class="mt-2 text-lg text-gray-500">
							A wonderful serenity has taken possession of my entire soul, like these sweet mornings
							of spring which I enjoy with my whole heart.
						</p>
					</div>
				</div>
			</div>
		</div>
	</section>

	<section class="flex justify-center">
		<div class="embed-responsive embed-responsive-16by9 w-8/12 overflow-hidden rounded ">
			<iframe
				class="embed-responsive-item h-96 w-full rounded"
				src="https://www.youtube.com/embed/v64KOxKVLVg"
				allowfullscreen
			/>
		</div>
	</section>

	<section>
		<div class="relative mx-auto w-full max-w-7xl items-center py-24 md:px-12 lg:px-16">
			<div class="divide-y overflow-hidden rounded-xl px-5 shadow-xl lg:px-0">
				<div class="flex w-full flex-wrap items-end justify-start bg-gray-50">
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<h2 class="mb-4 text-sm font-medium uppercase tracking-widest text-neutral-600">
								Sponsorships
							</h2>
							<ul class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<line x1="18" y1="6" x2="6" y2="18" />
											<line x1="6" y1="6" x2="18" y2="18" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</ul>
						</div>
					</div>
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<div class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</div>
						</div>
					</div>
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<div class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-normal tracking-tight text-gray-500"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-gray-300 text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</div>
						</div>
					</div>
					<div class="w-full md:w-1/4 lg:ml-auto xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<strong
								class="mx-auto flex items-end text-3xl font-black leading-none text-neutral-600"
							>
								<span>$10 </span>
							</strong>
							<div class="mt-2">
								<button
									role="button"
									class="block w-full transform items-center rounded-xl border-2 border-white bg-white px-10 py-3.5 text-center text-base font-medium text-blue-600 shadow-md transition duration-500 ease-in-out focus:outline-none focus:ring-2 focus:ring-gray-500 focus:ring-offset-2"
									>Buy Now</button
								>
							</div>
							<p class="mx-auto mt-6 text-xs text-gray-500">Only once within 6 months</p>
						</div>
					</div>
				</div>
				<div class="flex w-full flex-wrap items-end justify-start bg-white">
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<h2 class="mb-4 text-sm font-medium uppercase tracking-widest text-neutral-600">
								Sponsorships
							</h2>
							<ul class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</ul>
						</div>
					</div>
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<ul class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</ul>
						</div>
					</div>
					<div class="w-full md:w-1/4 xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<ul class="space-y-4">
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>Newsletter's Top.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1 Newsletter Issue.
								</li>
								<li
									class="mb-2 flex items-center text-base font-medium leading-relaxed text-neutral-600"
								>
									<span
										class="mr-2 inline-flex h-5 w-5 flex-shrink-0 items-center justify-center rounded-full bg-black text-white"
									>
										<svg
											fill="none"
											stroke="currentColor"
											stroke-linecap="round"
											stroke-linejoin="round"
											stroke-width="2.5"
											class="h-3 w-3"
											viewBox="0 0 24 24"
										>
											<path d="M20 6L9 17l-5-5" />
										</svg>
									</span>1.6k+ Readers.
								</li>
							</ul>
						</div>
					</div>
					<div class="w-full md:w-1/4 lg:ml-auto xl:w-1/4">
						<div class="relative flex h-full flex-col p-8">
							<strong class="mx-auto flex items-end text-3xl font-black leading-none text-blue-600">
								<span>$50 </span>
							</strong>
							<div class="mt-2">
								<button
									role="button"
									class="flex w-full transform items-center justify-center rounded-xl bg-blue-600 px-10 py-4 text-center text-base font-medium text-white transition duration-500 ease-in-out hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2"
									>Buy Now</button
								>
							</div>
							<p class="mx-auto mt-6 text-xs text-gray-500">Only once within 6 months</p>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</main>

<footer class="px-4 py-8 bg-gray-100" aria-labelledby="footer-heading">
	<div class="container flex flex-wrap items-center justify-center mx-auto space-y-4 sm:justify-between sm:space-y-0">
		<div class="flex flex-row pr-3 space-x-4 sm:space-x-8">
			<div class="flex items-center justify-center flex-shrink-0 w-12 h-12 rounded-full dark:bg-violet-400">
				<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" fill="currentColor" class="w-5 h-5 rounded-full dark:text-gray-900">
					<path d="M18.266 26.068l7.839-7.854 4.469 4.479c1.859 1.859 1.859 4.875 0 6.734l-1.104 1.104c-1.859 1.865-4.875 1.865-6.734 0zM30.563 2.531l-1.109-1.104c-1.859-1.859-4.875-1.859-6.734 0l-6.719 6.734-6.734-6.734c-1.859-1.859-4.875-1.859-6.734 0l-1.104 1.104c-1.859 1.859-1.859 4.875 0 6.734l6.734 6.734-6.734 6.734c-1.859 1.859-1.859 4.875 0 6.734l1.104 1.104c1.859 1.859 4.875 1.859 6.734 0l21.307-21.307c1.859-1.859 1.859-4.875 0-6.734z"></path>
				</svg>
			</div>
			<ul class="flex flex-wrap items-center space-x-4 sm:space-x-8">
				<li>
					<a rel="noopener noreferrer" href="#">Terms of Use</a>
				</li>
				<li>
					<a rel="noopener noreferrer" href="#">Privacy</a>
				</li>
			</ul>
		</div>
		<ul class="flex flex-wrap pl-3 space-x-4 sm:space-x-8">
			<li>
				<a rel="noopener noreferrer" href="#">Instagram</a>
			</li>
			<li>
				<a rel="noopener noreferrer" href="#">Facebook</a>
			</li>
			<li>
				<a rel="noopener noreferrer" href="#">Twitter</a>
			</li>
		</ul>
	</div>
</footer>
