<script>
  import MainLanding from "./sections/MainLanding.svelte";
  import WhatWeOffer from "./sections/WhatWeOffer.svelte";
  import JoinTheCommunity from "./sections/JoinTheCommunity.svelte";
  import Spacer from "./elements/Spacer.svelte";
</script>

<style>
  @import url("https://fonts.googleapis.com/css?family=Rubik:300,700&display=swap");

  :global(body) {
    padding: 0px;
    margin: 0px;
    background: #191928;
    -webkit-touch-callout: none; /* iOS Safari */
    -webkit-user-select: none; /* Safari */
    -khtml-user-select: none; /* Konqueror HTML */
    -moz-user-select: none; /* Old versions of Firefox */
    -ms-user-select: none; /* Internet Explorer/Edge */
    user-select: none; /* Non-prefixed version, currently
                                  supported by Chrome, Opera and Firefox */
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

</div>
