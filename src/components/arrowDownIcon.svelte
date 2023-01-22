
<script>
    let pageHeight = window.innerHeight;
</script>

<button class="ellipse" on:click={()=>window.scrollBy({top:pageHeight,behavior:'smooth'})}>
    <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
        <circle cx="20" cy="20" r="19.5" stroke="white" />
        <path
            d="M21 10C21 9.44772 20.5523 9 20 9C19.4477 9 19 9.44772 19 10H21ZM19.2929 30.7071C19.6834 31.0976 20.3166 31.0976 20.7071 30.7071L27.0711 24.3431C27.4616 23.9526 27.4616 23.3195 27.0711 22.9289C26.6805 22.5384 26.0474 22.5384 25.6569 22.9289L20 28.5858L14.3431 22.9289C13.9526 22.5384 13.3195 22.5384 12.9289 22.9289C12.5384 23.3195 12.5384 23.9526 12.9289 24.3431L19.2929 30.7071ZM19 10V30H21V10H19Z"
            fill="white"
        />
    </svg>
</button>

<style>
    @keyframes bounce {
        0% {
            transform: translateY(0px);
        }
        50% {
            transform: translateY(-8px);
        }
        0% {
            transform: translateY(0px);
        }
    }
    .ellipse {
        margin-top: 5rem;
        width: 60px;
        height: 60px;
        transition: 200ms;
        animation-name: bounce;
        animation-duration: 1.5s;
        animation-iteration-count: infinite;
        animation-timing-function: ease-in-out;
        cursor: pointer;
        background: transparent;
        border:none;
    }
</style>
