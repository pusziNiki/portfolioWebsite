<script>
  import CardImage from "./cardImage.svelte";
  import Image from "../assets/picture.jpg";

</script>
<header class="modal__title">Projects</header>
<div class="modal__body">
  <div class="modal__image">

    <CardImage alt="niki" image={"Image"}/>
  </div>
  <div class="modal__text">
    <span
      >Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias ipsum
      consequatur excepturi, nemo hic consequuntur eum suscipit nulla eaque
      dolorum architecto minima molestias ratione obcaecati tenetur voluptatem
      fugit vitae! Ducimus.</span
    >
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
