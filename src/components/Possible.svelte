<section class="container">
<h2>How is this all possible</h2>
<div class="containerForCon">
<h2>How Tracardi works?</h2>
<p>Tracardi <span class="orange"> collects events</span> that happen across multiple channels. Then is sends them to a visual editor where you can process it, orchestrate to other systems such as AI product referral systems, or interact with the user directly via micro front-ends</p>
<h2>How much does it costs? </h2>
<p>It is up to you. TRACARDI is a <span class="free"> free software</span> as long as you install it on premises and maintain it yourself. For cloud solutions please contact us.</p>
<h2 class="szer">Can i intergrate it on my old school web page? </h2>
<p>Sure. Integration is as simple as pasting a JavaScript code.</p>
</div>
<button class="yellowButoonQuest">I have more questions!</button>
</section>

<script>
    //tutaj będzie mapowanie przez tablice dla cystszego htmla
</script>

<style lang="scss">
.container{
    width: 100%;
    @include fc;
    flex-direction: column;
    h2{
        text-align: center;
        font-size:3rem;
        font-weight: bold;
    }
    .containerForCon{
        display: flex;
        flex-direction: column;
        margin-top: 10vh;
        width: 40%;
        p{
            margin-top: 5vh;
            text-align: left;
            line-height: 150%;
        }
        h2{
            text-align: left;
            font-size: 2.2rem;
            margin-top: 10vh;
            &:first-child{
                margin-top: 2vh;
            }
        }
        .szer{
            width: 120%;
        }
        .free{
            color: $blue;
        }
    }
    .yellowButoonQuest{
        margin-top: 15vh;
        width: 220px;
        height: 60px;
        margin-left: 25vw;
        border: none;
        background-color: $yellow;
        cursor: pointer;
        font-size: 15px;
        font-weight: bold;
    }
}

@media screen and (max-width: 800px) {
    .container 
    {
        .containerForCon 
        {
            width: 90%;
            margin: 0;
        }
    }
}
</style>