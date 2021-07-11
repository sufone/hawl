<script>
	let name = 'world';
	let persons = [
			{
				name: "Prophet Muhammad SAS",
				birthYear: 40,
				deathYear: 63,
			},
			{
				name: "Abu Bakr",
				birthYear: 3,
				deathYear: 65,
			},
		{
				name: "Omar",
				birthYear: 3,
				deathYear: 75,
			},
		{
				name: "Omar",
				birthYear: 3,
				deathYear: 75,
			},
		{
				name: "Omar",
				birthYear: 3,
				deathYear: 75,
			},
		]	
	console.log(persons)
	let margin = "20px"
</script>

<h1>Hello {name}!</h1>

<div id="container">
	<div id="wider">
		<div id="flex">
			{#each persons as person}
			<div id="main" style="margin-left: {person.birthYear}px; max-width:{(person.deathYear - person.birthYear) * 10}px">
				<p class="name-label">
					{person.name}
				</p>	
			</div>
		{/each}
		</div>
	</div>
</div>

<style>
	.name-label {
	overflow: visible;
	}
	#container {
		overflow-x: scroll;
		overflow-y: scroll;
		max-width: 100vw;
		min-height: 200px;
		max-height: 50vh;
		background-color: gray;
	}
	#main {
		background-color: blue;
		color: red;
	}
	#wider {
		width: 30000px;
		max-height: 30vh;
	display: flex;
		flex-direction: column;
		
	}
	#flex {
	
	}
</style>
