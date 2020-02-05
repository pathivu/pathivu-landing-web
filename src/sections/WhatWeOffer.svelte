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
	

    <LargeHeading beforeMarkedValue="What we" markedValue=" offer" afterMarkedValue="" textAlign="center"></LargeHeading>

	<Spacer></Spacer>

    <Paragraph content="Pathivu is powerful log ingestion and aggregation system. It's built from scratch by having cost-efficient and high write throughput in mind without trading log indexing."></Paragraph>
    
    <Spacer></Spacer>
    <Spacer></Spacer>

    <div class="buttons-group">
            
        <div class="button">
                
            <ButtonHolder buttonText="See All Features" backgroundColor="#1E2F3E" textColor="#00A8B0" buttonImage=""></ButtonHolder>
                
        </div>

        <div class="button">
                
            <ButtonHolder buttonText="Read about them on our blog" backgroundColor="#453331" textColor="#FF9A22" buttonImage=""></ButtonHolder>
                
        </div>

    </div>

</div>