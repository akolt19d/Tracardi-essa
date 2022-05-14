<section>
    <div class="transition">
        <Transition5 />
    </div>
    <div class="partner-opinion">
        IBM
    </div>
    <ul class="partner-list">
        {#each partners as partner}
            <li>
                <img src="./{partner}.png" alt={partner}>
            </li>
        {/each}
    </ul>
</section>

<script>
    import Transition5 from "./svg/transition5.svelte";

    const partners = ['ibm', 'mac-os-logo', 'windows']
</script>

<style lang="scss">
    section 
    {
        min-height: 60vh;
        width: 100%;
        background-color: #1C1818;
        margin: 25vh 0 15vh 0;
        position: relative;
        padding-top: 5vh;
        .transition
        {
            width: 100%;
            height: 50px;
            position: absolute;
            top: 0;
        }
        .partner-opinion 
        {
            width: 70rem;
            max-width: 90%;
            height: 30rem;
            background-color: $blue;
            margin: auto;
        }
        ul 
        {
            color: white;
            margin: 5rem auto;
            width: 30%;
            list-style-type: none;
            display: flex;
            justify-content: space-around;
            flex-direction: row;
            li 
            {
                img 
                {
                    height: 6rem;
                    filter: invert(100%);
                }
            }
        }
    }
</style>