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
    <ul>
        <li>
            Marthox
        </li>
        {#each routes as route}
            <li>
                <a href={route.url}>{route.name}</a>
            </li>
        {/each}
    </ul>
</nav>
