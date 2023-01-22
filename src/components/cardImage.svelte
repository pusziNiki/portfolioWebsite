<script>
    import { beforeUpdate } from "svelte";


    export let image;
    export let style = undefined;
    export let alt;
   
   beforeUpdate(() => {
   style = style || undefined
   })
</script>

<img class='image' style={style} alt={alt} src={image}>

<style>
    .image {
        width: inherit;
        height: inherit;
        overflow: hidden;
        overflow-clip-margin: 0px;
        border-radius: inherit;
    }
</style>
