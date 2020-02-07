<script>

    import LargeHeading from '../elements/LargeHeading.svelte';
    import ButtonHolder from '../elements/ButtonHolder.svelte';
    import Spacer from '../elements/Spacer.svelte';
    import Paragraph from '../elements/Paragraph.svelte';

</script>

<style>

    .bottom-landing{
		height: 100vh;
		width: 86vw;
        padding-left: 7vw;
        padding-right: 7vw;
		background: #191928;
	}

    .left{
        height: auto;
        width: 44%;
        position: relative;
        top: 0px;
        left: 0vw;
        margin-left: 7vw;
        display: inline-block;
    }

    .right{
        height: 100%;
        width: 46%;
        position: relative;
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
        float: left;
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
            margin-bottom: 15px;
        }

        .holder{
            transform: none;
            top: 40px;
        }

        img{
            height: 45px;
        }

        .laptop-landing{
            height: 100%;
            width: auto;
            top: 20%;
        }

    }

</style>


<div class="bottom-landing">
	
	<div class="left">
    
        <img class="laptop-landing" src="./images/laptop-landing.png" alt="">
    
    </div>

    <div class="right">

        <div class="holder">
        
            <LargeHeading beforeMarkedValue="Stay " markedValue=" informed" afterMarkedValue="" textAlign="left"></LargeHeading>

            <Spacer></Spacer>

            <Paragraph content="We'll be rolling out constant blogs and newsletters, stay connected and informed about Pathivu" textAlign="left"></Paragraph>

            <Spacer></Spacer>

            <div class="buttons-group">
            
                <div class="button">
                
                    <ButtonHolder buttonText="View Blog" backgroundColor="#453331" textColor="#FF9A22" buttonImage=""></ButtonHolder>
                
                </div>

                <div class="button">
                
                    <ButtonHolder buttonText="Subscribe to newsletter" backgroundColor="#16373D" textColor="#00AF81" buttonImage=""></ButtonHolder>
                
                </div>

            </div>
        
        </div>
    
    </div>


</div>