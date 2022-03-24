<nav>
    <ul>
        <li>Home</li>
        <li>How it works</li>
        <li>Contact</li>
        <li>Docs</li>
    </ul>
</nav>

<style lang="scss">
    nav
    {
        width: 100%;
        min-height: 12vh;
        @include fc;
        background: darken($bg-l, 1);
        margin: 0;
        transition: $theme-fade;
        position: fixed;
        top: 0;
        left: 0;
        z-index: 1000;
        ul 
        {
            display: flex;
            justify-content: space-evenly;
            list-style: none;
            li 
            {
                margin: 20px;
                font-weight: bold;
                font-size: 80%;
            }
        }
    }
    @media screen and (max-width: 600px) {
        nav 
        {
            display: none;
        }
    }
</style>