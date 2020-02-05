<script>
	
	import MainLanding from './sections/MainLanding.svelte';
	import WhatWeOffer from './sections/WhatWeOffer.svelte';
	import JoinTheCommunity from './sections/JoinTheCommunity.svelte';
	import Spacer from './elements/Spacer.svelte';


</script>

<style>

	@import url('https://fonts.googleapis.com/css?family=Rubik:300,700&display=swap');

	:global(body) {
        padding: 0px;
		margin: 0px;
		background: #191928;
	}

</style>

<div class="landing-holder">

	<MainLanding></MainLanding>

	<Spacer></Spacer>
	<Spacer></Spacer>
	<Spacer></Spacer>
	<Spacer></Spacer>

	<WhatWeOffer></WhatWeOffer>

	<Spacer></Spacer>
	<Spacer></Spacer>
	<Spacer></Spacer>
	<Spacer></Spacer>

	<JoinTheCommunity></JoinTheCommunity>

</div>