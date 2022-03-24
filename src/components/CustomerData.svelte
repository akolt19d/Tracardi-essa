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
        <div class="card">
            <h4>Frequency caps</h4>
            <p>
                Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.
            </p>
        </div>
        <div class="card">
            <h4>Frequency caps</h4>
            <p>
                Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.
            </p>
        </div>
        <div class="card">
            <h4>Frequency caps</h4>
            <p>
                Understand the number of emils reaching a customer every day & limit it to prevent unsubscribes.
            </p>
        </div>
    </div>
</section>
<div class="placeholder">
    <span></span>
</div>

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
                min-height: 22rem;
                border-radius: 2rem;
                padding: 2rem;
                text-align: center;
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
                        bottom: 3rem;
                        left: 2rem;
                    }
                }
            }
        }
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