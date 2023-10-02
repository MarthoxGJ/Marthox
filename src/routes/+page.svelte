<script>
    let page_header = "Hi, I'm Mateo... aka Marthox"
    let page_header_size = page_header.length
    let welcome_message = "welcome"
    let body_message = `I'm a software engineer from Colombia, currently working at <a href="https://inchcape.digital/" target="_blank">Inchcape Digital</a> as a full-stack developer`
</script>

<div class="landing-page-container">
    
    <div class="typewriter-container" style="--header-size: {page_header_size}">
        <h1 class="landing-page-header header-typewriting-animation">
            {page_header}
        </h1>
    </div>

    <div class="typewriter-container">
        <h1 class="landing-page-header welcome-typewriting-animation">
            {welcome_message}
        </h1>
    </div>

    <p class="body-container">
        {@html body_message}
    </p>
</div>

<style lang="scss">
    .typewriter-container {
        display: flex;
        padding: 2rem;
    }

    .body-container {
        font-family: monospace;
        font-size: 1rem;
        text-align: center;
        text-transform: uppercase;
        font-weight: 500;
        overflow: hidden;
        width: 40vw;
        opacity: 0;
        animation: appear 1s ease-in-out 4s forwards;
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
        white-space: nowrap;
        overflow: hidden;
    }
    
    .header-typewriting-animation {
        animation:
        typing 3s steps(var(--header-size))
    }
    
    .welcome-typewriting-animation {
        opacity: 0;
        animation: appear 1s ease-in-out 3s forwards;
    }
    
    @keyframes cursor {
        50% { border-color: transparent; }
    }
    
    @keyframes typing {
        from { width: 0 }
        to { width: 100% }
    }

    @keyframes appear {
        to {
            opacity: 1;
        }
    }
    
</style>
