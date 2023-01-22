<script>
    import ArrowDownIcon from "../components/arrowDownIcon.svelte";
    import "./name.css";
</script>

<div class="main-content">
    <h1>
        Hello!
        <br />
        I am <span class="name-gradient">Nikoletta Somogyi</span>,
        <br /> an aspiring UX/UI designer.
        <br />Scroll down to see my work!
    </h1>
    <div>
        <ul style="display: flex;">
            <li>Projects</li>
            <li>Other</li>
            <li>About Me</li>
        </ul>
    </div>
    <ArrowDownIcon />
</div>

<style>
    li {
        background-clip: text;
        -webkit-background-clip: text;
        
        text-align: left;
        list-style: none;
        padding: 1rem;
        padding-top: 0.5rem;
        padding-bottom: 0.5rem;
        font-size: 32px;
        font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS",
            sans-serif;
        margin-left: 3rem;
        margin-right: 3rem;
        border: 10px;
        background-image: linear-gradient(90deg, rgba(255, 0, 235, 1) 0%, rgba(0, 212, 255, 1) 100%);
        transition: 200ms ease-in-out;
        cursor: pointer;
    }
    li:hover {
        background: rgb(255, 0, 235);
        background: linear-gradient(
            90deg,
            rgba(255, 0, 235, 1) 0%,
            rgba(0, 212, 255, 1) 100%
        );
        -webkit-background-clip: text;
        background-clip: text;
        color: transparent;
        transform: scale(1.1);
    }
</style>
