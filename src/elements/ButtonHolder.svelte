<script>

    export let backgroundColor;
    export let textColor;
    export let buttonText;
    export let buttonImage;

</script>

<style>
    
    div{
        background: var(--buttonBackground);
        color: var(--textColor);
        padding-top: 10px;
        padding-bottom: 10px;
        padding-left: 30px;
        padding-right: 30px;
        width: auto;
        display: inline-block;
        border-radius: 4px;
        font-size: 18px;
        font-family: 'Rubik', sans-serif;
        font-weight: 300;
        letter-spacing: 1.2px;
        cursor: pointer;
    }

    img{
        height: 16px;
        width: auto;
        position: relative;
        top: 2px;
        margin-left: 10px;
    }

    @media(max-width:768px){
        div{
            font-size: 14px;
        }

        img{
            height: 12px;
            top:1px;
        }
    }

</style>

<div style="--buttonBackground:{backgroundColor};--textColor:{textColor};">

    {buttonText} {#if buttonImage!=""}<img src="{buttonImage}" alt="">{/if}
    
</div>

