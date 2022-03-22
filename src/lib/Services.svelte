<script>
    import { fly } from "svelte/transition"

    let descriptionActive = false
    let y;

    const toggleDescription = () => {
        descriptionActive = !descriptionActive
    }
</script>

<svelte:window bind:scrollY={y}/>

<section id="services">
    {#if y >= 450}
    <header>
        <h2>NUESTROS SERVICIOS</h2>
        <p>Full Wipe es la empresa líder en la realización de servicios de limpieza en los siguientes rubros</p>
    </header>
    <section class="services-container" transition:fly="{{ y: -100, duration: 1200 }}">
        <article class="item">
            <img src="/images/oficina.webp" alt="">
            <h2>Limpieza de Oficinas</h2>
            <div class={descriptionActive === true ? "description-overlay description-active" : "description-overlay"} on:mouseenter={toggleDescription} on:mouseleave={toggleDescription}>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-building-skyscraper" width="64" height="64" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <line x1="3" y1="21" x2="21" y2="21" />
                    <path d="M5 21v-14l8 -4v18" />
                    <path d="M19 21v-10l-6 -4" />
                    <line x1="9" y1="9" x2="9" y2="9.01" />
                    <line x1="9" y1="12" x2="9" y2="12.01" />
                    <line x1="9" y1="15" x2="9" y2="15.01" />
                    <line x1="9" y1="18" x2="9" y2="18.01" />
                  </svg>
                <p>Mesas, escritorios, bibliotecas, vidrios, alfombras, cristales, sillas, sillones, archivos, ceniceros, papeleros, la totalidad del mobiliario existente y los útiles de trabajo respectivos, serán repasados por nuestro personal usando elementos químicos de limpieza adecuados para cada caso.</p>
            </div>
        </article>
        <article class="item">
            <img src="/images/consorcio.webp" alt="">
            <h2>Limpieza de Consorcios</h2>
            <div class={descriptionActive === true ? "description-overlay description-active" : "description-overlay"} on:mouseenter={toggleDescription} on:mouseleave={toggleDescription}>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-building-community" width="64" height="64" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M8 9l5 5v7h-5v-4m0 4h-5v-7l5 -5m1 1v-6a1 1 0 0 1 1 -1h10a1 1 0 0 1 1 1v17h-8" />
                    <line x1="13" y1="7" x2="13" y2="7.01" />
                    <line x1="17" y1="7" x2="17" y2="7.01" />
                    <line x1="17" y1="11" x2="17" y2="11.01" />
                    <line x1="17" y1="15" x2="17" y2="15.01" />
                  </svg>
                <p>Palieres y pasillos serán barridos y lustrados con máquinas con cepillos y paños. Nuestro personal efectuara la limpieza a fondo de alfombras, lavado de vidrios y escaleras con agua jabonosa, procediéndose luego de la limpieza a su secado.
                    Los descansos, escalones y zócalos serán encerados y lustrados.</p>
            </div>
        </article>
        <article class="item">
            <img src="/images/industria.avif" alt="">
            <h2>Limpieza de Industrias</h2>
            <div class={descriptionActive === true ? "description-overlay description-active" : "description-overlay"} on:mouseenter={toggleDescription} on:mouseleave={toggleDescription}>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-building-factory" width="64" height="64" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M4 21c1.147 -4.02 1.983 -8.027 2 -12h6c.017 3.973 .853 7.98 2 12" />
                    <path d="M12.5 13h4.5c.025 2.612 .894 5.296 2 8" />
                    <path d="M9 5a2.4 2.4 0 0 1 2 -1a2.4 2.4 0 0 1 2 1a2.4 2.4 0 0 0 2 1a2.4 2.4 0 0 0 2 -1a2.4 2.4 0 0 1 2 -1a2.4 2.4 0 0 1 2 1" />
                    <line x1="3" y1="21" x2="22" y2="21" />
                  </svg>
                <p>Nuestro personal realiza el barrido, la limpieza de vidrios, aspirado de alfombras y lavado de pisos en las zonas de producción.
                    En aquellos mobiliarios que lo permitan se efectuara la limpieza según directivas de vuestra firma a fin de no dañar maquinarias ni equipos durante nuestro trabajo.</p>
            </div>
        </article>
        <article class="item">
            <img src="/images/comercio.webp" alt="">
            <h2>Limpieza de Comercios</h2>
            <div class={descriptionActive === true ? "description-overlay description-active" : "description-overlay"} on:mouseenter={toggleDescription} on:mouseleave={toggleDescription}>
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-building-store" width="64" height="64" viewBox="0 0 24 24" stroke-width="1.5" stroke="#ffffff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <line x1="3" y1="21" x2="21" y2="21" />
                    <path d="M3 7v1a3 3 0 0 0 6 0v-1m0 1a3 3 0 0 0 6 0v-1m0 1a3 3 0 0 0 6 0v-1h-18l2 -4h14l2 4" />
                    <line x1="5" y1="21" x2="5" y2="10.85" />
                    <line x1="19" y1="21" x2="19" y2="10.85" />
                    <path d="M9 21v-4a2 2 0 0 1 2 -2h2a2 2 0 0 1 2 2v4" />
                  </svg>
                <p>En los lugares cerrados la limpieza se efectuará con escobillón, pero adoptando siempre las precauciones necesarias para no levantar el polvo. A excepción de los muebles fijos, deberán ser corridos para limpiar debidamente el lugar que ocupen y luego deberán ser colocados nuevamente en su sitio.</p>
            </div>
        </article>
    </section>

    <button class="show-all-the-services">Ver todos los servicios</button>
    {/if}
</section>

<style>
    #services {
        min-height:105vh;
        max-width:100vw;
        background: url('/background_lines.png') no-repeat center center fixed;
        display:flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
        text-align: center;
    }

    header h2 {
        font-size:2rem;
    }

    header p {
        font-size:1.2rem;
    }

    .services-container {
        display:flex;
        align-items: center;
    }

    .item {
        min-width:20vw;
        height:45vh;
        text-align: center;
        display:flex;
        flex-direction: column;
        justify-content: space-evenly;
        margin:1.3rem;
    }

    .item h2 {
        font-size:1.65rem;
        font-weight:600;
        color:#000;
        background:#fff;
        border-radius: .8rem;
    }

    .item img {
        width:100%;
        height:17rem;
        object-fit: cover;
        border-radius: .5rem;
    }

    .description-overlay {
        position: absolute;
        width:20rem;
        height:45vh;
        background: rgba(87, 114, 255, 1);
        color:#f5f5f5;
        opacity:0;
        transition: all .5s ease;
        font-size:1.1rem;
        padding:.6rem;
        display:grid;
        place-items: center;
        border-radius: .8rem;
    }

    .description-overlay p {
        line-height: 1.7rem;
    }

    .description-active {
        opacity:1;
    }

    .show-all-the-services {
        border:none;
        background: #f5f5f5;
        outline:none;
        padding:1rem 4rem;
        border-radius: 1rem;
        font-size:1.1rem;
        border-bottom: 2px dashed rgb(87, 114, 255);
        border-top: 2px dashed rgb(87, 114, 255);
        border-right: 5px solid rgb(87, 114, 255);
        border-left: 5px solid rgb(87, 114, 255);
        text-transform: uppercase;
        cursor: pointer;
        transition: all .2s ease;
    }

    .show-all-the-services:hover {
        background: rgb(87, 114, 255);
        color:#f5f5f5;
    }

    @media screen and (max-width:1200px) {
        #services {
            height:auto;
            width:100vw;
            padding: 5vh 0;
        }

        header p {
            max-width:90vw;
        }

        .services-container {
            width:100vw;
            align-items: center;
            flex-direction: column;
        }

        .item {
            width:88vw;
            margin:1rem auto;
        }

        .show-all-the-services {
            padding: 1rem 2.8rem;
        }

        .description-overlay {
            padding:0;
        }

        .description-overlay p {
            padding:.3rem;
        }
    }
</style>
