<section>
    <div class="nocode-wrapper">
        <h3>NO CODE</h3>
        <p>NO CODE NO CODE NO CODE</p>
        <p>NO CODE NO CODE NO CODE</p>
    </div>
    <div class="inner-wrapper">

    </div>
</section>

<style lang="scss">
    section 
    {
        background-color: $yellow;
        min-height: 120vh;
        .inner-wrapper
        {
            min-height: 100vh;
            @include section-width;
        }
        .nocode-wrapper 
        {
            background-color: $orange;
            width: 50%;
            height: 60vh;
            @include fc;
            justify-content: end;
            flex-direction: column;
            font-weight: bold;
            overflow: hidden;
            line-height: 2.5rem;
            padding: 2rem 0 0 2rem;
            //color: white;
            h3
            {
                font-size: 400%;
                @include fc;
                height: 4rem;
            }
            p 
            {
                font-size: 270%;
                &:first-of-type
                {
                    transform: rotate(-90deg) translateY(1rem) translateX(-1rem);
                    transform-origin: left;
                }
            }
            h3, p 
            {
                background-image: linear-gradient(to right, white, white 55%, #111 55%, #111 80%, white 80%, white 95%, $yellow 95%);
                color: transparent;
                -webkit-background-clip: text;
                background-size: 100% 100%;
                animation: 1s nocode alternate infinite;
            }
        }
    }

    @keyframes nocode {
        0% 
        {
            background-position: left;
        }
        100% 
        {
            background-position: right;
        }
    }
</style>