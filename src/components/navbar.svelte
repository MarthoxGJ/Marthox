<script>
    /**
     * @type {Array<{name: string, url: string}>}
     */
    export let routes = [{
        name: "Home",
        url: "/"
    }, {
        name: "About",
        url: "/about"
    }, {
        name: "Contact",
        url: "/contact"}];
</script>

<nav>
    <li class="nav-logo">
        Marthox
    </li>
    <ul>
        {#each routes as route}
            <li class="nav-item">
                <a href={route.url}>{route.name}</a>
            </li>
        {/each}
    </ul>
    <li class="nav-language-selector">
        Language
    </li>
</nav>

<style lang="scss">
    nav {
        background-color: #333;
        color: #fff;
        display: flex;
        height: 3rem;
        justify-content: space-between;
    }

    ul {
        display: flex;
        justify-content: space-between;
    }

    li{
        display: flex;
        align-items: center;
        justify-content: center;
        width: 5rem;    
    }

    .nav-item {
        &:hover {
            background-color: #555;
        }
    }

    a {
        color: #fff;
        text-decoration: none;
    }
</style>
