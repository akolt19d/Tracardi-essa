<section>
    <div class="left-section">
        <div>
            <h3 class="orange">One API.</h3>
            <h3>Cleaner code.</h3>
            <p>
                Use <b><span class="orange">one API</span> to collect analytics data</b>, across any platform. We have SDKs for JavaScript, iOS, Android, and 20+ server-side languages.
            </p>
        </div>
        <div>
            <h4>Idea of reality in a few lines of code.</h4>
            <p>
                Functions is a new way to connect thousands of applications to Tracardi. With just ten lines of JavaScript, you can <b><span class="blue">build any integration</span> - no additional infrastructure required.</b>
            </p>
        </div>
    </div>
    <div class="right-section">
        <div class="buttons">
            <div>o</div>
            <div>m</div>
            <div>a</div>
            <div>g</div>
            <div>a</div>
            <div>d</div>
        </div>
        <div class="code">
            <code>
                <pre>
analytics.page(<span class="orange">'user-1023'</span>, <span class='orange'>'Home'</span>, &#123
    <span class='orange'>'title': 'Welcome | Initech',
    'url': 'http://www.example.com'</span> 
)&#125
                </pre>
            </code>
        </div>
    </div>
</section>

<script>
     import { fade } from 'svelte/transition';
	let visible = true; // jakiś fade na scroll 
</script>

<style lang="scss">
    section
    {
        min-height: 100vh;
        width: 100rem;
        margin: 10rem auto;
        max-width: 90vw;
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        .left-section
        {
            //background-color: aquamarine;
            border-right: 1px solid rgba($color: #000000, $alpha: .2);
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            flex-direction: column;
            div 
            {
                //background-color: red;
                width: 70%;
                aspect-ratio: 1/1;
                h3 
                {
                    font-size: 400%;
                }
                h4 
                {
                    font-size: 330%;
                }
                p 
                {
                    font-size: 120%;
                    line-height: 1.75;
                }
            }
        }
        .right-section
        {
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            flex-direction: column;
            transform: translateY(-9rem);
            .buttons 
            {
                width: 70%;
                display: grid;
                grid-template-columns: repeat(3, 1fr);
                grid-template-rows: repeat(2, 1fr);
                gap: 15px;
                div 
                {
                    //background-color: red;
                    aspect-ratio: 1/1;
                    box-shadow: 0 .5rem .75rem rgba($color: #000000, $alpha: .1);
                    border-radius: .5rem;
                    cursor: pointer;
                    @include fc;
                }
            }
            .code
            {
                width: 70%;
                aspect-ratio: 2/1;
                background-color: #111;
                color: lighten($blue, 40);
                @include fc;
                font-size: 150%;
                border-radius: .5rem;
            }
        }
    }
</style>