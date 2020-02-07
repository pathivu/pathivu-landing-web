<script>

    import LargeHeading from '../elements/LargeHeading.svelte';
    import ButtonHolder from '../elements/ButtonHolder.svelte';
    import Paragraph from '../elements/Paragraph.svelte';
    import Spacer from '../elements/Spacer.svelte';
    import InformationCard from '../elements/InformationCard.svelte';

    let allFeatures = false;
    let showAllOption = true;

    function allFeaturesToggle(event) {
        allFeatures = !allFeatures;
    }

    const mq = window.matchMedia("(min-width:768px)");

    if(mq.matches===true){
        allFeatures = true;
        showAllOption = false;
    }

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

    .card{
        margin-left: 40px;
        margin-right: 40px;
        display: inline-block;
    }

    .cards-holder{
        text-align: center;
    }

    @media(max-width:1200px){

        .button{
            display: block;
            margin-bottom: 20px;
            margin-right: 0px;
        }

        .card{
            margin-left: 40px;
            margin-right: 40px;
        }

    }

    @media(max-width:768px){

        .button{
            display: block;
            margin-bottom: 20px;
            margin-right: 0px;
        }

        .card{
            margin-left: 0px;
            margin-right: 0px;
        }

    }

</style>


<div class="main-landing" id="knowmore">
	

    <LargeHeading beforeMarkedValue="What we" markedValue=" offer" afterMarkedValue="" textAlign="center"></LargeHeading>

	<Spacer></Spacer>

    <Paragraph content="Pathivu is powerful log ingestion and aggregation system. It's built from scratch by having cost-efficient and high write throughput in mind without trading log indexing." textAlign="center"></Paragraph>
    
    <Spacer></Spacer>
    <Spacer></Spacer>
    
    <div class="cards-holder">
    
        <div class="card">
        
            <InformationCard iconColor="#FF9A22" iconBackgroundColor="#453331" paragraphText="A couple of line about the feature will help the person understand better" headingText="Fast ingestion" imageURL="./images/fast-ingestion.svg"></InformationCard>
        
        </div>

        <div class="card">
        
            <InformationCard iconColor="#B931FF" iconBackgroundColor="#421F5F" paragraphText="A couple of line about the feature will help the person understand better" headingText="Powerful query analysis" imageURL="./images/powerful-query-analysis.svg"></InformationCard>
        
        </div>
    
        {#if allFeatures===true}

            <div class="card">
        
                <InformationCard iconColor="#FF424C" iconBackgroundColor="#442635" paragraphText="A couple of line about the feature will help the person understand better" headingText="Log indexing" imageURL="./images/log-indexing.svg"></InformationCard>
            
            </div>
        
            <div class="card">
            
                <InformationCard iconColor="#00A8B0" iconBackgroundColor="#1E2F3E" paragraphText="A couple of line about the feature will help the person understand better" headingText="Log tailing" imageURL="./images/log-tailing.svg"></InformationCard>
            
            </div>
 
            <div class="card">
            
                <InformationCard iconColor="#00AF81" iconBackgroundColor="#16373D" paragraphText="A couple of line about the feature will help the person understand better" headingText="Cost efficient" imageURL="./images/cost-efficient.svg"></InformationCard>
            
            </div>

            <div class="card">
            
                <InformationCard iconColor="#EB0098" iconBackgroundColor="#401D41" paragraphText="A couple of line about the feature will help the person understand better" headingText="Beautiful dashboard" imageURL="./images/beautiful-dashboard.svg"></InformationCard>
            
            </div>

        {/if}

    </div>

    <Spacer></Spacer>
    <Spacer></Spacer>

    <div class="buttons-group">

        {#if showAllOption === true}

            {#if allFeatures===false}
            
                <div class="button" on:click={allFeaturesToggle}>
                        
                    <ButtonHolder buttonText="See All Features" backgroundColor="#1E2F3E" textColor="#00A8B0" buttonImage=""></ButtonHolder>
                        
                </div>

            {/if}

            {#if allFeatures===true}
                
                <div class="button" on:click={allFeaturesToggle}>
                        
                    <ButtonHolder buttonText="Show less features" backgroundColor="#1E2F3E" textColor="#00A8B0" buttonImage="" action="#"></ButtonHolder>
                        
                </div>

        {/if}

        {/if}

        <div class="button">
                
            <ButtonHolder buttonText="Read about them on our blog" backgroundColor="#453331" textColor="#FF9A22" buttonImage="" action="https://blog.pathivu.io"></ButtonHolder>
                
        </div>

    </div>

</div>