<section class="container">
    <div class="ConForCol">
        <h2>Launch with the right stack</h2>
        <p>Enable the best product analytics tools, A/B testing tools, and data warehousing tools with the flip of a switch.</p>
        <div>Tutaj będzie obrazek</div>
        <button>Explore</button>
    </div>
    
</section>
<script>

</script>
<style lang="scss">
    .container{
        width: 100%;
        margin-top: 35vh;
        .ConForCol{
            display: flex;
            align-items: center;
            width: 100%;
            flex-direction: column;
            h2{
                font-size: 3rem;
                color: $blue
            }
            p{
                width: 32%;
                text-align: center;
                margin-top: 5vh;
                font-size: 18px;
            }
            div{
                width: 30%;
                height: 40vh;
                background-color: black;
                color: white;
                margin-top: 12vh;
                text-align: center;
                position: relative;
                &::before{
                 width: 60%;
                 height: 10vh;
                 margin-top: 25%;
                 margin-left: -40%;
                 display: block;
                 position: absolute;
                 background: linear-gradient(0deg, rgba(55, 121, 239, 0.34), rgba(55, 121, 239, 0.34)), rgba(55, 121, 239, 0.34);
                 z-index: -1;
                 content: '';
                }
            }
            button{
                width: 18vw;
                height: 8vh;
                margin-top: 10vh;
                border: none;
                color: white;
                background-color: $blue;
                cursor: pointer;
                font-size: 18px;
                font-weight: bold;
                position: relative;
                transition: .2s;
                &::after{
                    content: '';
                    background: linear-gradient(0deg, rgba(55, 121, 239, 0.34), rgba(55, 121, 239, 0.34)), rgba(55, 121, 239, 0.34);
                    z-index: -1;
                    width: 18vw;
                    height: 8vh;
                    display: block;
                    position: absolute;
                    left: 15%;
                    top: 35%;
                }
                &:hover{
                    transform: scale(1.05);
                }
            }
        }
    }
</style>