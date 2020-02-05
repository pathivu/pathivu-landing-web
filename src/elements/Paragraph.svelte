<script>

    export let content;

</script>

<style>
    
    div{
        font-size: 16px;
        width: 85vw;
        font-family: 'Rubik', sans-serif;
        font-weight: 300;
        letter-spacing: 1.8px;
        color: #ffffff;
        line-height: 30px;
        text-align: var(--textAlign);
        margin:auto auto;
        max-width: 800px;
        text-align: center;
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

<div>{content}</div>

