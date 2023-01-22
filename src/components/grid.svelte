
<div class="grid-container">
    <slot></slot>
</div>

<style>
   .grid-container {
  display: grid;
  grid-template-columns: repeat(12, 2fr);
  grid-column-gap: 30px;
  grid-row-gap: 30px;

}
</style>
