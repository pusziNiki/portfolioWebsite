<script>
    import { beforeUpdate } from "svelte";


    export let width = undefined;
    beforeUpdate(()=> {
        width = width || 12
    })

   

</script>



<div class="item" style="--width:{width}" >
    <slot />
</div>

<style>
    .item {
        grid-column: span var(--width);
        display: inline;
    }
</style>
