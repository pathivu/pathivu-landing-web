<script>
  import MainLanding from "./sections/MainLanding.svelte";
  import WhatWeOffer from "./sections/WhatWeOffer.svelte";
  import JoinTheCommunity from "./sections/JoinTheCommunity.svelte";
  import Spacer from "./elements/Spacer.svelte";
  import BottomLanding from "./sections/BottomLanding.svelte";
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Nunito:300,700&display=swap');

  :global(body) {
    padding: 0px;
    margin: 0px;
    background: #191928;
    -webkit-touch-callout: none;
    -webkit-user-select: none;
    -khtml-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
  }

</style>

<div class="landing-holder">

  <MainLanding />

  <Spacer />
  <Spacer />
  <Spacer />
  <Spacer />

  <WhatWeOffer />

  <Spacer />
  <Spacer />
  <Spacer />
  <Spacer />

  <JoinTheCommunity />

  <Spacer />
  <Spacer />
  <Spacer />
  <Spacer />

  <BottomLanding />

</div>
