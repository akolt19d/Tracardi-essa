<footer>
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
                    ooomagad
                </h5>
                <li>'essa'</li>
                <li>'essa'</li>
                <li>'essa'</li>
            </ul>
            <ul class="ul-wrapper">
                <h5>
                    ooomagad
                </h5>
                <li>'essa'</li>
                <li>'essa'</li>
                <li>'essa'</li>
            </ul>
            <ul class="ul-wrapper">
                <h5>
                    ooomagad
                </h5>
                <li>'essa'</li>
                <li>'essa'</li>
                <li>'essa'</li>
            </ul>
        </div>
        <div>
            <h3>ooomagad</h3>
            <h6>essa</h6>
        </div>
    </div>
    <div class="end">
        <ul class="tos">
            <li>essa</li>
            <li>essa</li>
            <li>essa</li>
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
        background-color: #152543;
        margin-top: 20vh;
        color: $bg-l;
        width: 100vw;
        padding: 8rem;
        padding-bottom: 3rem;
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
                background: rgba($color: #fff, $alpha: .05);
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
                }
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
        }
    }
</style>