<script lang="ts">
	import '../app.css';
	const data = [
		{
			rank: 1,
			lastName: 'Doe',
			age: 25,
		},
		{
			rank: 2,
			lastName: 'Doedkhjbfgkjhdfdjkhjk',
			age: 23,
		},
		{
			rank: 3,
			lastName: 'Smith',
			age: 30,
		},
		{
			rank: 4,
			lastName: 'Smith',
			age: 28,
		},
	];
</script>

<div
	class="flex min-h-screen items-center justify-center bg-black font-sans text-white"
>
	<table class="table rounded bg-dark text-left">
		<thead>
			<tr>
				<th
					class="pl-8 pt-9 text-sm font-extralight leading-3 text-secondary subpixel-antialiased"
					>RANKiNg</th
				>
				<th
					class="pl-8 pt-9 text-sm font-extralight leading-3 text-secondary subpixel-antialiased"
					>MEMBER</th
				>
				<th
					class="pl-8 pt-9 text-sm font-extralight leading-3 text-secondary subpixel-antialiased"
					>HOURS</th
				>
				<th
					class="px-8 pt-9 text-sm font-extralight leading-3 text-secondary subpixel-antialiased"
					>SCORE</th
				>
			</tr>
		</thead>
		<tbody>
			{#each data as person}
				<tr>
					<td>{person.rank} <span> arrow</span></td>
					<td>{person.lastName}</td>
					<td>{person.age}</td>
				</tr>
			{/each}
		</tbody>
	</table>
</div>
