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

    .para{
        margin: auto auto;
    }

    @media(max-width:1200px){

        .button{
            display: block;
            margin-bottom: 20px;
            margin-right: 0px;
        }

    }

    @media(max-width:768px){

        .button{
            display: block;
            margin-bottom: 20px;
            margin-right: 0px;
        }

    }

</style>


<div class="main-landing">
	

    <LargeHeading beforeMarkedValue="Join the" markedValue=" community" afterMarkedValue="" textAlign="center"></LargeHeading>

	<Spacer></Spacer>

    <div class="para">
    
        <Paragraph content="We love the people who love us, come spread love <3" textAlign="center"></Paragraph>
    
    </div>
    
    <Spacer></Spacer>
    <Spacer></Spacer>

    <div class="buttons-group">
            
        <div class="button">
                
            <ButtonHolder buttonText="Join the channel" backgroundColor="#252941" textColor="#7289DA" buttonImage="./images/discord.svg" action="https://discordapp.com/invite/m5hZbPv"></ButtonHolder>
                
        </div>

        <div class="button">
                
            <ButtonHolder buttonText="Follow us" backgroundColor="#19273D" textColor="#1DA1F2" buttonImage="./images/twitter.svg" action="https://www.twitter.com/PathivuHQ"></ButtonHolder>
                
        </div>

        <div class="button">
                
            <ButtonHolder buttonText="View On GitHub" backgroundColor="#2F2F3D" textColor="#FFFFFF" buttonImage="./images/github.svg" action="https://www.github.com/pathivu/pathivu"></ButtonHolder>
                
        </div>

    </div>

</div>