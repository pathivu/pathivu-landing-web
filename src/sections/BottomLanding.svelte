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
        height: 100%;
        width: 44%;
        position: relative;
        display: inline-block;
        overflow: hidden;
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
        float: left;
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
    }

    @media(max-width:1200px){

        .button{
            display: block;
            text-align: center;
            margin-bottom: 15px;
        }

    }

    @media(max-width:768px){

        .bottom-landing{
            height: auto;
        }

        .right{
            width: 100%;
            height: 320px;
        }

        .left{
            width: 100%;
            height: auto;
        }

        .button{
            display: block;
            text-align: center;
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
            width:60%;
            height: auto;
            position: relative;
            top: 0%;
            left: 50%;
            transform: translate(-50%,-0%);
        }

    }

</style>


<div class="bottom-landing">
	
	<div class="left">
    
        <img class="laptop-landing" src="./images/phone-pathivu.png" alt="">
    
    </div>

    <div class="right">

        <div class="holder">
        
            <LargeHeading beforeMarkedValue="Stay " markedValue=" informed" afterMarkedValue="" textAlign="left"></LargeHeading>

            <Spacer></Spacer>

            <Paragraph content="We'll be rolling out constant blogs and newsletters, stay connected and informed about Pathivu" textAlign="left"></Paragraph>

            <Spacer></Spacer>

            <div class="buttons-group">
            
                <div class="button">
                
                    <ButtonHolder buttonText="View Blog" backgroundColor="#453331" textColor="#FF9A22" buttonImage="" action="https://blog.pathivu.io/"></ButtonHolder>
                
                </div>

                <div class="button">
                
                    <ButtonHolder buttonText="Subscribe to newsletter" backgroundColor="#16373D" textColor="#00AF81" buttonImage="" action="https://newsletter.pathivu.io"></ButtonHolder>
                
                </div>

            </div>
        
        </div>
    
    </div>


</div>