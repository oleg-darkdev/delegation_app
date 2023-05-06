<script>
	import { boards } from '../../../lib/shared/';

	let selectedBoard = boards[0],
		start = false;
</script>

<section class="flex w-full justify-center py-4">
	<div
		class="{start
			? 'hidden'
			: ''} flex max-w-lg flex-col rounded-lg border border-gray-200 bg-white p-4 text-gray-500 shadow-md dark:border-gray-700 dark:bg-gray-800 dark:text-gray-400 sm:p-8"
	>
  		<div class="stats shadow max-w-xs mb-4 mx-auto stats-vertical lg:stats-horizontal ">
			<div class="stat place-items-center">
				<div class="stat-title">Tasks Delegated</div>
				<div class="stat-value">34</div>
			</div>

			<div class="stat place-items-center">
				<div class="stat-title">Not delegated</div>
				<div class="stat-value text-secondary">12</div>
			</div>
		</div>
		<div class="mb-6">
			<div class="mb-4 flex items-center justify-between">
				<span class="text-sm text-gray-500">Last updates: {selectedBoard.lastUpd}</span>
				<a href="/" class="text-sm font-medium text-gray-100 hover:underline ">Trello board </a>
			</div>

			<p class="mt-3 text-lg font-medium leading-6">
				{selectedBoard.title}
			</p>
			<p class="mt-2 text-lg text-gray-500">
				{selectedBoard.description}
			</p>
		</div>


		<div class="mb-4 flex items-center justify-between">
			<h5 class="text-xl font-bold leading-none text-gray-900 dark:text-white">Board Members</h5>
			<a href="/" class="text-sm font-medium text-blue-600 hover:underline dark:text-blue-500"
				>View all
			</a>
		</div>
		<ul
			class="divide-y divide-gray-200 rounded-lg border border-0 border-gray-200 bg-white text-gray-500 dark:divide-gray-600 dark:border-gray-700 dark:bg-gray-800 dark:!bg-transparent dark:text-gray-400"
		>
			{#each selectedBoard.members as member}
				<li class="w-full py-2 px-4 text-sm font-medium first:rounded-t-lg last:rounded-b-lg">
					<div class="flex items-center space-x-4">
						<img
							alt={member.nickname}
							src={member.avatar}
							class="h-10 w-10 flex-shrink-0 rounded-full bg-gray-100 text-gray-600 dark:bg-gray-600 dark:text-gray-300"
						/>
						<div class="min-w-0 flex-1">
							<p class="truncate text-sm font-medium text-gray-900 dark:text-white">
								{member.nickname}
							</p>
							<p class="truncate text-sm text-gray-500 dark:text-gray-400">{member.email}</p>
						</div>
						<div
							class="inline-flex items-center text-base font-semibold text-gray-900 dark:text-white"
						>
							{member.status}
						</div>
					</div>
				</li>
			{/each}
		</ul>

		<button
			on:click={() => (start = !start)}
			class="btn-md btn mx-auto my-2 max-w-xs font-medium text-blue-600 hover:text-blue-500"
		>
			Start to delegation
		</button>
	</div>

	<div class={start ? 'max-w-4xl overflow-x-auto' : 'hidden'}>
		<table class="table w-full">
			<!-- head -->
			<thead>
				<tr>
					<th>
						<label>
							<input type="checkbox" class="checkbox" />
						</label>
					</th>
					<th>Name</th>
					<th>Job (ID)</th>
					<th>Delegation</th>
					<th />
				</tr>
			</thead>
			<tbody>
				<tr>
					<th>
						<label>
							<input type="checkbox" class="checkbox" />
						</label>
					</th>
					<td>
						<div class="flex items-center space-x-3">
							<div class="avatar">
								<div class="mask mask-squircle h-12 w-12">
									<img
										src=""
										alt="Avatar Tailwind CSS Component"
									/>
								</div>
							</div>
							<div>
								<div class="font-bold">Yancy Tear</div>
								<div class="text-sm opacity-50">Brazil</div>
							</div>
						</div>
					</td>
					<td>
						Wyman-Ledner (#Trello_card_ID)
						<br />
						<span class="badge-ghost badge badge-sm">Community Outreach Specialist</span>
					</td>
					<td class='text-center'>20%</td>
					<th>
						<button class="btn-ghost btn-xs btn">details</button>
					</th>
				</tr>
			</tbody>
			<!-- foot -->
			<tfoot>
				<tr>
					<th />
					<th>Name</th>
					<th>Job (ID)</th>
					<th>Delegation</th>
					<th />
				</tr>
			</tfoot>
		</table>
	</div>
</section>
