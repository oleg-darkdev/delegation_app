<script>
  	import { boards } from '../../lib/shared/';

	$: showApp = false;
</script>

<!--class={showApp ? 'hidden' : ''}-->
<!-- {#if !showApp} -->
<section class:hidden={showApp}>
	<div class="min- flex flex-col justify-center py-12 sm:px-6 lg:px-8">
		<div class="sm:mx-auto sm:w-full sm:max-w-md">
			<h2 class="mt-6 text-center text-3xl font-extrabold text-neutral-600">
				Sign in to your account
			</h2>
		</div>

		<div class="mt-8 sm:mx-auto sm:w-full sm:max-w-md">
			<div class="px-4 py-8 sm:px-10">
				<!-- <form class="space-y-6" action="#" method="POST"> -->
				<div class="space-y-6">
					<div>
						<label for="email" class="block text-sm font-medium text-gray-700">
							Email address
						</label>
						<div class="mt-1">
							<input
								id="email"
								name="email"
								type="email"
								autocomplete="email"
								required=""
								class="block w-full transform rounded-lg border border-transparent bg-gray-50 px-5 py-3 text-base text-neutral-600 placeholder-gray-300 transition duration-500 ease-in-out focus:border-transparent focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-300"
							/>
						</div>
					</div>

					<div>
						<label for="password" class="block text-sm font-medium text-gray-700"> Password </label>
						<div class="mt-1">
							<input
								id="password"
								name="password"
								type="password"
								autocomplete="current-password"
								required=""
								class="block w-full transform rounded-lg border border-transparent bg-gray-50 px-5 py-3 text-base text-neutral-600 placeholder-gray-300 transition duration-500 ease-in-out focus:border-transparent focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-300"
							/>
						</div>
					</div>

					<div class="flex items-center justify-between">
						<div class="flex items-center">
							<input
								id="remember-me"
								name="remember-me"
								type="checkbox"
								class="h-4 w-4 rounded border-gray-300 text-blue-600 focus:ring-blue-500"
							/>
							<label for="remember-me" class="ml-2 block text-sm text-neutral-600">
								Remember me
							</label>
						</div>

						<div class="text-sm">
							<a href=''

								class="font-medium text-blue-600 hover:text-blue-500"
							>
								Forgot your password?
            </a>
						</div>
					</div>

					<div>

						<button
            type="submit"
              on:click={() => (showApp = !showApp)}
							class="flex w-full transform items-center justify-center rounded-xl bg-blue-600 px-10 py-4 text-center text-base font-medium text-white transition duration-500 ease-in-out hover:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2"
							>Sign in</button
						>
					</div>
					<!-- </form> -->
				</div>
			</div>
		</div>
	</div>
</section>


<section class:hidden={!showApp} class="flex  w-full justify-center py-12">
	<div class="relative">
		<div class="relative flex justify-start">
			<span class="bg-white pr-3 text-lg font-medium text-neutral-600"> All Boards</span>
		</div>
	</div>

	<div class="flex flex-row flex-wrap justify-center space-y-8">
		{#each boards as board}
			<a href="/app/board/"
				><div class="group max-w-lg pt-8 sm:flex lg:items-end">
					<div class="mb-4 flex-shrink-0 sm:mb-0 sm:mr-4">
						<img
							class="h-32 w-full rounded-md object-cover lg:w-32"
							src="https://i.pinimg.com/originals/f6/41/af/f641af4abaf0416c0142f4ee6ab32348.jpg"
							alt="Image text"
						/>
					</div>
					<div>
						<span class="text-sm text-gray-500">Last updates: {board.lastUpd}</span>
						<p class="mt-3 text-lg font-medium leading-6">
							{board.title}
						</p>
						<p class="mt-2 text-lg text-gray-500">
							{board.description}
						</p>
						<div class="ml-2 flex">
							{#each board.members as member}
								<img
									alt={member.nickname}
									src={member.avatar}
									class="-ml-4 h-10 w-10 rounded-full border-2 border-white bg-gray-100 text-gray-600 dark:border-gray-800 dark:bg-gray-600 dark:text-gray-300"
								/>
							{/each}
							<a
								href="/"
								class="relative -ml-4 flex h-10 w-10 items-center justify-center rounded-full border-2 border-white bg-gray-100 bg-gray-700 text-sm text-gray-600 text-white hover:bg-gray-600 dark:border-gray-800 dark:bg-gray-600 dark:text-gray-300"
								>{board.members.length}
							</a>
						</div>
					</div>
				</div>
			</a>
		{/each}
	</div>
</section>
