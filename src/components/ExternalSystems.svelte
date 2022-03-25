<section class="container">
    <h2>INTERGRATE EXTERNAL   <span class="white">   SYSTEMS</span></h2>
    <div class="blueSquare"></div>
    <div class="containerForContent">
        <div class="conForText">
            <p class="fat">Use the <span class="blue">social media, SaaS, AI</span> to boost your sales. Integrate any system with your e-commerce solution.</p>
            <p class="small">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,</p>
        </div>
    </div>
</section>
<style lang="scss">
    .container{
        width: 100%;
        margin-top: 10vh;
        position: relative;
        h2{
            font-size: 4rem;
            text-align: center;
            .white{
                color: white !important;
            }
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
                }
                .fat{
                    font-weight: bold;
                    margin-bottom: 3.3rem;
                    .blue{
                        color: $blue;
                    }
                }
            }
        }
        .blueSquare{
            position: absolute;
            width: 350px;
            height: 130px;
            z-index: -1;
            background-color: $blue;
            right: 12.3vw;
            top: 0;
        }
    }
</style>