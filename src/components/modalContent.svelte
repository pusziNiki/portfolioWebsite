<script>
  import CardImage from "./cardImage.svelte";
  import Image from "../assets/picture.jpg";
  export let title;
  export let image;
  export let imageAltText;
  export let description;
  export let link;

</script>
<header class="modal__title">{title}</header>
<div class="modal__body">
  <div class="modal__image">

    <CardImage alt={imageAltText} image={image}/>
  </div>
  <div class="modal__text">
    <p>{description}</p>
    <a href={link}>View project!</a>
  </div>
</div>

<style>

  .modal__body {
    display: flex;
  }

  .modal__image {
    flex: 1;
  }

  .modal__text {
    flex: 1;
    display: grid;
    place-items: center;
    font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS",
      sans-serif;
    font-size: 20px;
    color: rgb(186, 186, 186);
  }

  .modal__title {
    font-size: 24px;
    font-family: Gill;
    text-align: center;
    margin-bottom: 2rem;
    color: aliceblue;
  }
</style>
