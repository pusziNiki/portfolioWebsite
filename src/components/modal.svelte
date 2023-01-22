<script>
    export let visible = false;
    export let showModal;

</script>

<div class="modal" style="display: {visible ? 'flex' : 'none'}">
    <div class="modal__content">
            <button class="closeContent" on:click={() => showModal = false}>
    <svg
      width="22"
      height="22"
      viewBox="0 0 22 22"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path d="M1.5 21L21.3848 1" stroke="white" stroke-linecap="round" />
      <path d="M20.5 21L1 1" stroke="white" stroke-linecap="round" />
    </svg>
  </button>
        <slot />
    </div>
</div>

<style>
    .modal {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background: rgba(0, 0, 0, 0.5);
        z-index: 1000;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .modal__content {
        position: relative;
        width: 90vw;
        height: 90vh;
        background: rgba(23, 23, 23, 0.97);
        padding: 1rem;
        box-shadow: 0 0 10px 3px rgba(0, 0, 0, 0.1);
        border-radius: 5px;
    }
          .closeContent {
        border: none;
        background-color: transparent;
        position: absolute;
        top: 0;
        right: 0;
        padding: 1rem;
        cursor: pointer;
    }

</style>
