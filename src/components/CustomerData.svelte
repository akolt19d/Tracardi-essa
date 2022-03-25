<section>
    <div class="cd-text">
        <h3>What is <span class="blue">customer data?</span></h3>
        <p>
            Every marketing and analytics app runs on the same three types of data: who your users are, what they are doing, and where are they whilst doing it. Collect it once with Tracardi and send it to any tool.
        </p>
    </div>
    <div>
        <hr>
        <hr>
    </div>
    <div class="cards">
        
        {#each tabOfData as item}
        <div class="card">
            <svg class="svgCom" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d={item.pathToSvg}/></svg>
            <h4>{item.title}</h4>
            <p>
                {item.Text}
            </p>
        </div>
            
        {/each}
    </div>
</section>
<div class="placeholder">
    <span></span>
</div>

<script>
    const tabOfData = [
    {
        title: "Frequency caps",
        Text: "Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.",
        pathToSvg: "M0 128C0 92.65 28.65 64 64 64H448C483.3 64 512 92.65 512 128V384C512 419.3 483.3 448 448 448H64C28.65 448 0 419.3 0 384V128zM48 128V150.1L220.5 291.7C241.1 308.7 270.9 308.7 291.5 291.7L464 150.1V127.1C464 119.2 456.8 111.1 448 111.1H64C55.16 111.1 48 119.2 48 127.1L48 128zM48 212.2V384C48 392.8 55.16 400 64 400H448C456.8 400 464 392.8 464 384V212.2L322 328.8C283.6 360.3 228.4 360.3 189.1 328.8L48 212.2z",
    },
    {
        title: "Frequency caps",
        Text: "Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.",
        pathToSvg: "M500.3 443.7l-119.7-119.7c27.22-40.41 40.65-90.9 33.46-144.7C401.8 87.79 326.8 13.32 235.2 1.723C99.01-15.51-15.51 99.01 1.724 235.2c11.6 91.64 86.08 166.7 177.6 178.9c53.8 7.189 104.3-6.236 144.7-33.46l119.7 119.7c15.62 15.62 40.95 15.62 56.57 0C515.9 484.7 515.9 459.3 500.3 443.7zM79.1 208c0-70.58 57.42-128 128-128s128 57.42 128 128c0 70.58-57.42 128-128 128S79.1 278.6 79.1 208z",
    },
    {
        title: "Frequency caps",
        Text: "Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.",
        pathToSvg: "M112.1 454.3c0 6.297 1.816 12.44 5.284 17.69l17.14 25.69c5.25 7.875 17.17 14.28 26.64 14.28h61.67c9.438 0 21.36-6.401 26.61-14.28l17.08-25.68c2.938-4.438 5.348-12.37 5.348-17.7L272 415.1h-160L112.1 454.3zM192 0C90.02 .3203 16 82.97 16 175.1c0 44.38 16.44 84.84 43.56 115.8c16.53 18.84 42.34 58.23 52.22 91.45c.0313 .25 .0938 .5166 .125 .7823h160.2c.0313-.2656 .0938-.5166 .125-.7823c9.875-33.22 35.69-72.61 52.22-91.45C351.6 260.8 368 220.4 368 175.1C368 78.8 289.2 .0039 192 0zM288.4 260.1c-15.66 17.85-35.04 46.3-49.05 75.89h-94.61c-14.01-29.59-33.39-58.04-49.04-75.88C75.24 236.8 64 206.1 64 175.1C64 113.3 112.1 48.25 191.1 48C262.6 48 320 105.4 320 175.1C320 206.1 308.8 236.8 288.4 260.1zM176 80C131.9 80 96 115.9 96 160c0 8.844 7.156 16 16 16S128 168.8 128 160c0-26.47 21.53-48 48-48c8.844 0 16-7.148 16-15.99S184.8 80 176 80z"  
    }
]
    
</script>


<style lang="scss">
    section 
    {
        position: relative;
        @include section-width;
        .cd-text 
        {
            max-width: 33rem;
            margin: auto;
            h3 
            {
                text-align: center;
                font-weight: bold;
                font-size: 200%;
                margin-bottom: 2rem;
            }
        }
        div 
        {
            margin: 3rem 0 5rem 0;
            hr 
            {
                margin: .5rem auto;
                height: 5px;
                background-color: black;
                color: black;
                &:last-child 
                {
                    width: 5rem;
                }
            }
        }
        .cards
        {
            @include fc;
            flex-wrap: wrap;
            p 
            {
                margin-bottom: 2rem;
            }
            .card 
            {
                margin: .5rem;
                width: 18rem;
                min-height: 18rem;
                border-radius: 2rem;
                padding: 2rem;
                text-align: center;
                h4{
                    margin-bottom: 2rem;
                    font-size: 20px;
                }
                &:nth-child(2)
                {
                    position: relative;
                    background: $yellow;
                    &::after
                    {
                        content: '';
                        width: calc(100% - 4rem);
                        height: 5px;
                        background: black;
                        position: absolute;
                        bottom: 2rem;
                        border-radius: 2px;
                        left: 2rem;
                    }
                }
            }
        }
    }
    .svgCom{
        width: 4.5rem;
        margin-bottom: 10px;
    }
    .placeholder 
    {
        position: relative;
        height: 40vh;
        span 
        {
            display: block;
            background-color: $yellow;
            width: 100vw;
            height: 5rem;
            position: absolute;
            bottom: 0;
            left: 0;
            box-shadow: 0px -15px 15px rgba($color: #000000, $alpha: 0.2), 0px -2rem 0 darken($orange, 10);
        }
    }
</style>