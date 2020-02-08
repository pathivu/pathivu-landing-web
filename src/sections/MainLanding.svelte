<script>

    import LargeHeading from '../elements/LargeHeading.svelte';
    import ButtonHolder from '../elements/ButtonHolder.svelte';
    import Spacer from '../elements/Spacer.svelte';

    const mq = window.matchMedia("(min-width:768px)");

</script>

<style>

    .main-landing{
		height: 100vh;
		width: 86vw;
        padding-left: 7vw;
        padding-right: 7vw;
		background: #191928;
	}

    .left{
        height: auto;
        width: 44%;
        position: absolute;
        top: 0px;
        left: 0vw;
        margin-left: 7vw;
        display: inline-block;
    }

    .right{
        height: 100%;
        width: 56%;
        position: absolute;
        top: 0px;
        right: 0px;
        display: inline-block;
        overflow: hidden;
    }

    .holder{
        height: auto;
        position: relative;
        top: 50vh;
        transform: translateY(-50%);
    }

    .button{
        display: inline;
        margin-right: 30px;
    }

    img{
        height: 60px;
        width: auto;
    }

    .laptop-landing{
        width: 80%;
        height: auto;
        position: relative;
        top: 15%;
        float: right;
    }

    .bottom-button{
        display: block;
        position: absolute;
        top:100vh;
        left: 50%;
        transform: translateY(-200%)translateX(-50%);
        width: 100%;
        text-align: center;
    }

    @media(max-width:1200px){

        .button{
            display: block;
            margin-bottom: 15px;
        }

        .laptop-landing{
            top: 30%;
        }

    }

    @media(max-width:768px){

        .right{
            height: 25%;
            width: 100%;
        }

        .left{
            width: 86vw;
            height: auto;
            top: 30%;
            left: 0px;
            margin-left: 0px;
            padding-left: 7vw;
            padding-right: 7vw;
        }

        .button{
            display: block;
            margin: auto auto;
            margin-bottom: 15px;
            text-align:center;
        }

        .holder{
            transform: none;
            top: 40px;
        }

        img{
            height: 45px;
            position: relative;
            left:50%;
            transform: translateX(-50%);
        }

        .laptop-landing{
            height: 90%;
            width: auto;
            top: 20%;
            margin:auto auto;
            float: none;
        }

    }

</style>


<div class="main-landing">
	
	<div class="left">
    
        <div class="holder">

            <img src="./images/pathivu-logo.svg" alt="">

            <Spacer></Spacer>
        
            <LargeHeading beforeMarkedValue="An" markedValue=" efficient" afterMarkedValue=" log aggregation system" textAlign="left"></LargeHeading>

            <Spacer></Spacer>

            <div class="buttons-group">

                <div class="button">
                
                    <ButtonHolder buttonText="View On GitHub" backgroundColor="#2F2F3D" textColor="#FFFFFF" buttonImage="./images/github.svg" action="https:/github.com/pathivu/pathivu"></ButtonHolder>
                
                </div>

            </div>
        
        </div>
    
    </div>

    <div class="right">
    
        {#if mq.matches===true}

            <img class="laptop-landing" src="./images/laptop-landing.png" alt="">

        {/if}

        {#if mq.matches===false}

            <img class="laptop-landing" src="./images/laptop-landing-mobile.png" alt="">

        {/if}
    
    </div>

    <div class="bottom-button">
    
        <ButtonHolder buttonText="Know More" backgroundColor="" textColor="#00A8B0" buttonImage="./images/down-arrow.svg" action="#knowmore"></ButtonHolder>
    
    </div>


</div>