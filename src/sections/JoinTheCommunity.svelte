<script>

    import LargeHeading from '../elements/LargeHeading.svelte';
    import ButtonHolder from '../elements/ButtonHolder.svelte';
    import Paragraph from '../elements/Paragraph.svelte';
    import Spacer from '../elements/Spacer.svelte';

</script>

<style>

    .main-landing{
		height: auto;
		width: 100vw;
		background: #191928;
	}    

    .button{
        display: inline;
        margin-right: 30px;
    }

    .buttons-group{
        text-align: center;
    }

    @media(max-width:1200px){

        .button{
            display: block;
            margin-bottom: 15px;
        }

    }

    @media(max-width:768px){

        .button{
            display: block;
            margin-bottom: 15px;
        }

    }

</style>


<div class="main-landing">
	

    <LargeHeading beforeMarkedValue="Join the" markedValue=" community" afterMarkedValue="" textAlign="center"></LargeHeading>

	<Spacer></Spacer>

    <Paragraph content="We love the people who love us, come spread love <3"></Paragraph>
    
    <Spacer></Spacer>
    <Spacer></Spacer>

    <div class="buttons-group">
            
        <div class="button">
                
            <ButtonHolder buttonText="See All Features" backgroundColor="#252941" textColor="#7289DA" buttonImage="./images/discord.svg"></ButtonHolder>
                
        </div>

        <div class="button">
                
            <ButtonHolder buttonText="Follow Us" backgroundColor="#19273D" textColor="#1DA1F2" buttonImage="./images/twitter.svg"></ButtonHolder>
                
        </div>

        <div class="button">
                
            <ButtonHolder buttonText="View On GitHub" backgroundColor="#2F2F3D" textColor="#FFFFFF" buttonImage="./images/github.svg"></ButtonHolder>
                
        </div>

    </div>

</div>