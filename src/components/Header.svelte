<header>
    <p>
        Tracardi is an open-source <span class="blue">customer data platform</span> to help you engage your customers and build your sales through automated digital experiences.
    </p>
    <div>
        <h1>TRACARDI</h1>
        <input type="email" placeholder="Enter your email">
        <button>Get Started</button>
    </div>
    <video autoplay muted loop src={`./Comp_2.webm`}></video>
</header>

<style lang="scss">
    header
    {
        min-height: 100vh;
        @include fc;
        @include section-width;
        text-align: center;
        overflow-x: hidden;
        div 
        {
            z-index: 2;
            position: absolute;
            transform: translateY(-15vh);
            h1  
            {
                color: $blue;
                font-size: 4.4rem;
            }
            input 
            {
                outline: none;
                padding: .8rem 1.8rem;
                background: darken($bg-l, 1);
                border: 0;
                border-radius: .125rem;
                box-shadow: -.25rem -.25rem .5rem white, .25rem .25rem .5rem rgba($color: #000000, $alpha: 0.1);
                text-align: center;
                transition: $theme-fade, .3s transform, .3s box-shadow;
                &::placeholder
                {
                    font-weight: bold;
                }
            }
            button 
            {
                padding: .8rem 1.8rem;
                background: $orange;
                border: 0;
                border-radius: .125rem;
                color: $bg-l;
                font-weight: bold;
                box-shadow: -.2rem -.2rem .5rem white, .2rem .2rem .5rem rgba($color: #000000, $alpha: 0.05);
                margin-left: 1rem;
                @include button-effects;
            }
        }
        video
        {
            position: absolute;
            top: 40vh;
            width: 70vw;
        }
        p 
        {
            z-index: 2;
            position: relative;
            bottom: 10rem;
            font-size: 90%;
            font-weight: 500;
            transform: translateY(-12vh);
        }
    }
</style>