<script>
    import "./projects.css";
    import Card from "../components/card.svelte";
    import CardImage from "../components/cardImage.svelte";
    import Grid from "../components/grid.svelte";
    import GridItem from "../components/gridItem.svelte";
    import Image from "../assets/picture.jpg";
    import Modal from "../components/modal.svelte";
    import ModalContent from "../components/modalContent.svelte";
    let showModal = false;
</script>

<div class="main-content">
    <h2>Projects</h2>
    <Grid>
        <GridItem width="4">
            <Card onClick={() => (showModal = true)}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
        <GridItem width="4">
            <Card onClick={() => console.log()}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
        <GridItem width="4">
            <Card onClick={() => console.log()}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
        <GridItem width="4">
            <Card onClick={() => console.log()}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
        <GridItem width="4">
            <Card onClick={() => console.log()}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
        <GridItem width="4">
            <Card onClick={() => console.log()}>
                <CardImage alt="niki" image={Image} />
            </Card>
        </GridItem>
    </Grid>
    <Modal bind:visible={showModal} bind:showModal={showModal }>
        <ModalContent />
    </Modal>
</div> 
