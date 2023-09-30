<script>
    let page_header = "Hi, I'm Mateo... aka Marthox."
    let page_header_size = page_header.length
</script>

<div class="landing-page-container" style="--header-size: {page_header_size}">
    <div class="typewriter-container">
        <h1 class="landing-page-header">
            {page_header}
        </h1>
    </div>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
</div>

<style lang="scss">
    .typewriter-container {
        display: flex;
        padding: 2rem;
    }

    .landing-page-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        position: absolute;
        z-index: -1;
        width: 100vw;
        height: 100vh;
        top: 0;
        left: 0;
    }

    .landing-page-header {
        font-family: monospace;
        font-size: 2rem;
        text-align: center;
        letter-spacing: 10px;
        text-transform: uppercase;
        font-weight: 1000;
        border-right: 0.2rem solid #333;
        white-space: nowrap;
        overflow: hidden;
        animation:
            typing 3s steps(var(--header-size)),
            cursor 0.4s step-end infinite alternate;
    }

    @keyframes cursor {
        50% { border-color: transparent; }
    }

    @keyframes typing {
        from { width: 0 }
        to { width: 100% }
    }

</style>
