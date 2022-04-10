<script>
    let navActive = false;

    function toggleNav() {
        navActive = !navActive;
    }

    function closeNav() {
        navActive = false;
    }
</script>

<header class="app_header">
    <section class="logo">
            <img src="/images/logo.png" alt="">
    </section>

    <nav class={navActive === true ? "navigation active" : "navigation"}>
        <ul>
            <li><a href="#hero" on:click={closeNav}>Inicio</a></li>
            <li><a href="#services" on:click={closeNav}>Servicios</a></li>
            <li><a href="#responsabilities" on:click={closeNav}>Responsabilidad</a></li>
            <li><a href="#materials" on:click={closeNav}>Materiales</a></li>
            <li><a href="#CV" on:click={closeNav}>CV</a></li>
            <li><a href="#contact" on:click={closeNav}>Contacto</a></li>
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
            <p class="number">223 4 246659</p>
        </section>
    </nav>

    <button class="burger" on:click={toggleNav}>
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-menu-2" width="32" height="32" viewBox="0 0 24 24" stroke-width="1.5" stroke="#000000" fill="none" stroke-linecap="round" stroke-linejoin="round">
            <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
            <line x1="4" y1="6" x2="20" y2="6" />
            <line x1="4" y1="12" x2="20" y2="12" />
            <line x1="4" y1="18" x2="20" y2="18" />
        </svg>
    </button>
</header>

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
        height:14vh;
        background-color: #f5f5f5;
        display:flex;
        justify-content:space-around;
        align-items:center;
        box-shadow:0 0 10px var(--secondary);
    }

    /* DANGER */

    img {
        height: 20vh;
    }

    /* DANGER */

    .navigation {
        display:flex;
    }

    .phone-number {
        display: flex;
        align-items: center;
        font-size:1.3rem;
        color:var(--primary);
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
        background-color:var(--primary);
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
            margin-left: 3rem;
        }

        .burger {
            display:flex;
            padding:0 4rem;
        }

        .navigation {
            position:fixed;
            z-index:7;
            top:12vh;
            left:0;
            display:flex;
            height:88vh;
            width:75vw;
            background:#f5f5f5;
            flex-direction: column;
            justify-content: space-evenly;
            align-items: center;
            transition: all .2s ease;
            transform: translateX(-120%);
        }

        .active {
            transform: translateX(0);
        }

        ul {
            flex-direction: column;
        }

        li {
            margin: .8rem 0;
            font-size: 1.25rem;
        }

        .number {
            font-size:1.4rem;
        }
    }
</style>
