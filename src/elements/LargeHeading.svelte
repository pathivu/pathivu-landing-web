<script>

    export let beforeMarkedValue;
    export let markedValue;
    export let afterMarkedValue;
    export let textAlign;

</script>

<style>
    
    div{
        font-size: 3.3vw;
        font-family: 'Nunito', sans-serif;
        font-weight: 700;
        letter-spacing: 4.2px;
        color: #ffffff;
        text-align: var(--textAlign);
    }

    span{
        color: #00A8B0;
    }

    @media (max-width:758px){
        div{
            font-size: 20px;
            line-height: 40px;
        }
    }

</style>

<div style="--textAlign:{textAlign}">{beforeMarkedValue}<span>{markedValue}</span>{afterMarkedValue}</div>

