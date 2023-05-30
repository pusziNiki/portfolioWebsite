<script>
    import Card from "./card.svelte";
    import CardImage from "./cardImage.svelte";
    import GridItem from "./gridItem.svelte";
    import Modal from "./modal.svelte";
    import ModalContent from "./modalContent.svelte";
    export let title;
    export let description;
    export let image;
    export let imageAltText;
    export let link;
    let showModal = false;
</script>


<GridItem width="4">
    <Card onClick={() => (showModal = true)}>
        <CardImage alt="niki" image={Image} />
    </Card>
</GridItem>
<Modal bind:visible={showModal} bind:showModal={showModal }>
    <ModalContent description={description} title={title} image={image} imageAltText={imageAltText} link={link}/>
</Modal>