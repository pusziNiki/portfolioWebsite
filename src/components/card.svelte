<script>
    import { beforeUpdate } from "svelte";


    export let onClick = undefined;
    beforeUpdate(() => (onClick = onClick || undefined));
</script>


<div class="card" on:click={onClick} style="--cursor{onClick? "pointer": "default"};">
    <slot />
</div>

<style>
    .card {
        cursor: pointer;
        width: 100%;
        height: 100%;
        background-color: #343434;
        border-radius: 5px;
        box-shadow: 2px 2px 10px rgba(138, 138, 138, 0.183);
        transition: 200ms;
    }
    .card:hover{
        /* transform: rotate(720deg); */
        transform: scale(1.05)
    }


</style>
