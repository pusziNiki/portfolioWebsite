<script>
    import "./projects.css";
    import Card from "../components/card.svelte";
    import CardImage from "../components/cardImage.svelte";
    import Grid from "../components/grid.svelte";
    import GridItem from "../components/gridItem.svelte";
    import Image from "../assets/picture.jpg";
    import Modal from "../components/modal.svelte";
    import ModalContent from "../components/modalContent.svelte";
    import Project from "../components/project.svelte";
    let showModal = false;

    const projects = [
        {
            title: "SecondChance",
            description: "this is a test",
            image: "",
            imageAltText: "SecondChance",
            link: "",

        },
        {
            title: "SecondChance",
            description: "this is a test",
            image: "",
            imageAltText: "SecondChance",
            link: "",

        },
        
    ]
</script>



<div class="main-content">
    <h2>Projects</h2>
    <Grid>
        {#each projects as project}
        <Project description={project.description} image={project.image} imageAltText={project.imageAltText} link={project.link} title={project.title} />
        {/each}
    </Grid>
      
</div> 
