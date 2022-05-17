<script>
    import Transition from './svg/transition4.svelte'
</script>

<footer>
    <div class="transition">
        <Transition />
    </div>
    <div class="headline">
        <h3>TRACARDI</h3>
        <div>
            <input type="email" placeholder="Your work email">
            <button>
                See how it works
            </button>
        </div>
    </div>
    <div class="contact">
        <div class="inner-wrapper">
            <ul class="ul-wrapper">
                <h5>
                    navigation
                </h5>
                <li>Home</li>
                <li>How it works</li>
                <li>Contact</li>
            </ul>
            <ul class="ul-wrapper">
                <h5>
                    for clients
                </h5>
                <li>Documentation</li>
                <li>Open source</li>
                <li>Our team</li>
            </ul>
            <ul class="ul-wrapper">
                <h5>
                    support
                </h5>
                <li>Help center</li>
                <li>Contact us</li>
            </ul>
        </div>
        <div>
            <h3>ourgmail@gmail.com</h3>
            <h6>Tracardi</h6>
        </div>
    </div>
    <div class="end">
        <ul class="tos">
            <li>Privacy policy</li>
            <li>Terms of service</li>
            <li>Website data connection</li>
        </ul>
        <ul class="icons">
            <li>X</li>
            <li>X</li>
            <li>X</li>
            <li>X</li>
        </ul>
    </div>
</footer>

<style lang="scss">
    footer 
    {
        font-size: 160%;
        color: $bg-l;
        width: 100vw;
        padding: 8rem;
        padding-bottom: 3rem;
        position: relative;
        overflow-x: hidden;
        .transition 
        {
            // position: absolute;
            // top: 0;
            // left: 0;
            width: 100%;
            height: 10vh;
        }
        .headline
        {
            margin: 5rem 0;
            display: flex;
            justify-content: space-between;
            h3 
            {
                font-size: 6rem;
            }
            input 
            {
                outline: none;
                padding: 1.4rem 2rem;
                background: rgba($color: #fff, $alpha: .95);
                border: 0;
                border-radius: 1rem;
                text-align: center;
                transition: $theme-fade, .3s transform, .3s box-shadow;
                box-shadow: 0 .2rem .6rem rgba($color: #000000, $alpha: .2);
                font-size: 80%;
                &::placeholder
                {
                    font-weight: bold;
                    color: rgba($color: #000000, $alpha: .55)
                }
            }
            button 
            {
                padding: 1.4rem 2rem;
                background: 0;
                box-shadow: 0 0 0 .05rem $yellow;
                border: 0;
                border-radius: 1rem;
                color: $bg-l;
                font-weight: bold;
                margin-left: 1rem;
                font-size: 80%;
                color: $yellow;
                transition: .3s background, .3s color, .3s transform, .3s box-shadow;
                cursor: pointer;
                &:hover, &:focus
                {
                    box-shadow: 0 0 0 .05rem #111;
                    background: #111;
                    color: white;
                    transform: scale(0.97);
                }
                &:active 
                {
                    transform: scale(0.94);
                }
            }
        }
        .contact    
        {
            margin: 4rem 0;
            display: flex;
            justify-content: space-between;
            .inner-wrapper 
            {
                display: flex;
                justify-content: space-between;
                width: 50%;
                .ul-wrapper
                {
                    list-style: none;
                    * 
                    {
                        margin: 3rem 0;
                    }
                    h5 
                    {
                        color: $yellow;
                    }
                }
            }
            div:last-child 
            {
                opacity: 50%;
            }
        }
        .end 
        {
            margin-top: 7rem;
            display: flex;
            justify-content: space-between;
            * 
            {
                display: flex;
            }
            .icons 
            {
                color: $yellow;
            }
        }
    }

    @media screen and (max-width: 800px) {
        footer 
        {
            padding: 0;
            .headline 
            {
                margin: 2rem 0;
                flex-direction: column;
                h3 
                {
                    width: 100%;
                    text-align: center;
                    font-size: 200%;
                }
                div 
                {
                    @include fc;
                    flex-direction: column;
                    *
                    {
                        margin: .5rem 0;
                    }
                }
            }
            .contact 
            {
                align-items: center;
                flex-direction: column;
                text-align: center;
                margin: 1rem 0;
                .inner-wrapper 
                {
                    flex-wrap: wrap;
                    justify-content: center;
                    width: 100%;
                    margin-bottom: 1rem;
                    .ul-wrapper
                    {
                        margin: 0 1rem;
                        * 
                        {
                            margin: 1rem 0;
                        }
                    }
                }
                div:last-child 
                {
                    @include fc;
                    flex-direction: column-reverse;
                }
            }
            .end 
            {
                margin-top: 2rem;
                flex-direction: column;
                align-items: center;
            }
        }
    }
</style>