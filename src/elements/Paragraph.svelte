<script>

    export let content;
    export let textAlign;

</script>

<style>
    
    div{
        font-size: 16px;
        width: 85%;
        font-family: 'Nunito', sans-serif;
        font-weight: 300;
        letter-spacing: 1.8px;
        color: #ffffff;
        line-height: 30px;
        max-width: 800px;
        text-align: var(--textAlign);
    }

    span{
        color: #00A8B0;
    }

    @media (max-width:758px){
        div{
            font-size: 10px;
            line-height: 20px;
        }
    }

</style>



{#if textAlign === 'left'}

<div style="--textAlign:{textAlign};">{content}</div>

{/if}

{#if textAlign === 'center'}
<div style="--textAlign:{textAlign};;margin:auto auto;">{content}</div>

{/if}