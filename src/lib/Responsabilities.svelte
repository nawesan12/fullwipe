<section id="responsabilities">
    <section class="container">
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
        <article class="item">
            <div class="logo">
                <svg></svg>
                <h4></h4>
            </div>
            <p></p>
        </article>
    </section>
</section>

<style>
    #responsabilities {
        height:105vh;
        width:100vw;
        background: url('/clouds.svg') repeat bottom center;
        display:grid;
        place-items: center;
    }

    .container {
        width:75vw;
        height:70vh;
        background:#f5f5f5;
        border-radius: 2rem;
        box-shadow: 0 0 10px #222;
        display:flex;
        justify-content: space-evenly;
        align-items: center;
        gap: 1rem;
    }

    @media screen and (max-width:1200px) {
        #responsabilities {
            height:auto;
            padding:3vh 0 10vh;
            background-position: right center;
        }

        .container {
            width:85vw;
            height:auto;
            flex-wrap: wrap;
            align-items: center;
            justify-content: unset;
            flex-direction: column;
            border-radius: 1rem;
        }
    }
</style>