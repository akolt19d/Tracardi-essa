<script>
    import Transition from './svg/transition3.svelte'
</script>

<section class="container">
    <div class="transition">
        <Transition />
    </div>
    <div class="conForData">
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
        <div>
            <h2>Siema1</h2>
            <p> Lorem ipsum dolor sit amet consectetur adipisicing elit. Vero non nisi ullam modi? Optio quas repellendus dicta voluptas recusandae quod!</p>
        </div>
    </div>
</section>

<style lang="scss">
    .container{
        width: 100%;
        background: #3B78ED;
        min-height: 80vh;
        margin-top: 12rem;
        padding: 5rem 0;
        position: relative;
        background-color: $blue;
        .transition 
        {
            position: absolute;
            left: 0;
            top: 0;
            background: white;
            width: 100%;
            height: 22vh;
        }
        .conForData{
            display: flex;
            width: 80%;
            min-height: 60vh;
            margin: 3rem 10%;
            flex-wrap: wrap;
            justify-content: center;
            //@include fc;
            gap: 3rem 1.75rem;
            div{
                flex-basis: 26%;
                min-width: 30rem;
                //margin: 5rem 0;
                background-color: darken($blue, 8);
                padding: 20px;
                align-items: center;
                display: flex;
                flex-direction: column;
                z-index: 1;
                h2{
                    margin-top: 2vh;
                }
                p{
                    margin-top: 5vh;
                    width: 70%;
                    text-align: justify;
                    color: rgba(255, 255, 255, 0.56);
                }
            }
        }   
    }
</style>