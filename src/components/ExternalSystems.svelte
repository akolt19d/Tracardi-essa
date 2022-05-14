<script>
    import Transition2 from './svg/transition2.svelte'
</script>

<section class="container">
    <div class="transition">
        <Transition2 />
    </div>
    <h2>INTERGRATE EXTERNAL   <span class="white">   SYSTEMS</span></h2>
    <div class="containerForContent">
        <div class="conForText">
            <p class="fat">Use the <span class="blue">social media, SaaS, AI</span> to boost your sales. Integrate any system with your e-commerce solution.</p>
            <p class="small">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,</p>
            <a href="/">Explore Tracardi for external systems.</a>
        </div>
    </div>
</section>

<style lang="scss">
    .container{
        width: 100%;
        //margin-top: 10vh;
        position: relative;
        .transition
        {
            height: 45vh;
            position: relative;
        }
        h2{
            font-size: 4rem;
            text-align: center;
        }
        .containerForContent{
            display: flex;
            justify-content: flex-end;
            .conForText{
                display: flex;
                margin-right: 16rem;
                flex-basis: 25%;
                line-height: 140%;
                align-self: right;
                flex-direction: column;
                margin-top: 200px;
                text-align: justify;
                font-size: 18px;
                .small{
                    color: grey;
                    margin-bottom: 3.3rem;
                }
                .fat{
                    font-weight: bold;
                    margin-bottom: 3.3rem;
                    .blue{
                        color: $blue;
                    }
                }
                a 
                {
                    color: $blue;
                }
            }
        }
    }

    @media screen and (max-width: 800px) {
        .container 
        {
            .transition 
            {
                height: 15vh;
            }
            h2 
            {
                font-size: 220%;
            }
            .containerForContent
            {
                justify-content: center;
                flex-direction: column-reverse;
                align-items: center;
                .conForText
                {
                    margin: 0 !important;
                    max-width: 90%;
                    width: 30rem;
                    font-size: 100%;
                }
            }
        }
    }
</style>