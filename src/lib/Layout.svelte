<script>

</script>

<header class="app_header">
    <section class="logo">
        <div class="content">
            <span>Full <br> Wipe</span>
        </div>
    </section>

    <nav class="navigation">
        <ul>
            <li><a href="#hero">Inicio</a></li>
            <li><a href="#services">Servicios</a></li>
            <li><a href="#responsabilities">Responsabilidad</a></li>
            <li><a href="#materials">Materiales</a></li>
            <li><a href="#CV">CV</a></li>
            <li><a href="#contact">Contacto</a></li>
        </ul>
        <section class="phone-number">
            <span class="number-logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-device-mobile" width="36" height="36" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5773ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <rect x="7" y="4" width="10" height="16" rx="1" />
                    <line x1="11" y1="5" x2="13" y2="5" />
                    <line x1="12" y1="17" x2="12" y2="17.01" />
                </svg>
            </span>
            <p class="number">223 5 929292</p>
        </section>
    </nav>

    

    <button class="burger">
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-menu-2" width="32" height="32" viewBox="0 0 24 24" stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
            <line x1="4" y1="6" x2="20" y2="6" />
            <line x1="4" y1="12" x2="20" y2="12" />
            <line x1="4" y1="18" x2="20" y2="18" />
        </svg>
    </button>
</header>

<main>
    <slot></slot>
</main>

<footer class="app_footer">

</footer>

<style>
    @keyframes hoverItemUnderlined {
        from {
            opacity:0;
            width:0;
        }

        to {
            opacity:1;
            width:100%;
        }
    }

    .app_header {
        max-width:100vw;
        height:12vh;
        background-color: #f5f5f5;
        display:flex;
        justify-content:space-around;
        align-items:center;
    }

    /* DANGER */

    .content {
        position: absolute;
        background:#000;
        color:#fff;
        top:0;
        height:15vh;
        z-index:10;
        padding:1rem 2rem 0;
        display:grid;
        place-items: center;
        text-align: center;
        font-size: 1.7rem;
        font-weight: bold;
        line-height: 2.7rem;
    }

    /* DANGER */

    .navigation {
        display:flex;
    }

    .phone-number {
        display: flex;
        align-items: center;
        font-size:1.3rem;
        color:rgb(87, 114, 255);
    }

    .number-logo {
        margin: 0 .8rem;
    }

    ul {
        list-style:none;
        display:flex;
        align-items: center;
    }

    li {
        font-size:1.2rem;
        margin: 0 1rem;
    }

    li::after {
        content:'';
        margin:5px 0 0;
        display:block;
        width:0;
        height:2px;
        background-color:rgb(87, 114, 255);
        transition:width .3s ease-in-out;
    }

    li:hover::after {
        animation: hoverItemUnderlined .5s;
    }

    a {
        text-decoration: none;
    }

    .burger {
        border:none;
        background:none;
        outline:none;
        cursor:pointer;
        display:none;
    }

    @media screen and (max-width:1200px) {
        .app_header {
            max-width: 100vw;
            justify-content: space-between;
        }

        .content {
            margin-left: 2rem;
        }

        .burger {
            display:flex;
            padding:0 4rem;
        }

        .navigation {
            position:fixed;
            top:12vh;
            left:0;
            display:block;
        }

        ul {
            flex-direction: column;
        }
    }
</style>