<script>

    export let iconBackgroundColor;
    export let iconColor;
    export let headingText;
    export let paragraphText;
    export let imageURL;

</script>

<style>
    
    .holder{
        width: 360px;
        text-align: center;
        height: 270px;
        margin: auto auto;
        font-family: 'Rubik', sans-serif;
    }

    .icon-part{
        height: 60px;
        width: 60px;
        background:var(--iconBackgroundColor);
        display: block;
        z-index: 99;
        position: relative;
        top: 0px;
        left: 40px;
        border-radius: 6px;
    }

    .text-part{
        padding-left: 40px;
        padding-right: 40px;
        padding-top:60px;
        padding-bottom: 40px;
        background: blue;
        position: absolute;
        margin-top: -30px;
        background: #222231;
        border-radius: 4px;
    }

    .text-holder{
        width: 280px;
    }

    h1{
        padding: 0px;
        margin: 0px;
        margin-bottom: 15px;
        font-weight: 700;
        font-size: 18px;
        letter-spacing: 2px;
        text-align: left;
        width: 100%;
        color: var(--iconColor);
    }

    p{
        padding: 0px;
        margin: 0px;
        font-weight: 300;
        font-size: 12px;
        letter-spacing: 1.4px;
        color:#FFFFFF;
        text-align: left;
        width: 100%;
        line-height: 25px;
    }

    img{
        width: 24px;
        height: 24px;
        object-fit: 100% auto;
        position: relative;
        top:50%;
        transform: translateY(-50%); 
    }

    @media(max-width:600px){
        .text-holder{
            width: 220px;
        }

        .holder{
            width: 300px;
        }

        .icon-part{
            left: 0px;
            margin: auto auto;
        }

        h1,p{
            text-align: center;
        }
    }
    

</style>

<div class="holder">

    <div class="icon-part" style="--iconBackgroundColor:{iconBackgroundColor};">
    
        <img src="{imageURL}" alt="">
    
    </div>

    <div class="text-part">
    
        <div class="text-holder">
        
            <h1 style="--iconColor:{iconColor};">{headingText}</h1>
            <p>{paragraphText}</p>

        </div>
    
    </div>

</div>

