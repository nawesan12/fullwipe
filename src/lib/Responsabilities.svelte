<script>
    import { fly } from "svelte/transition";

    let y
</script>

<svelte:window bind:scrollY={y} />

<section id="responsabilities">
    {#if y >= 2215}
    <section class="container" transition:fly="{{ y: -100, duration: 1200 }}">
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-atom" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <line x1="12" y1="12" x2="12" y2="12.01" />
                    <path d="M12 2a4 10 0 0 0 -4 10a4 10 0 0 0 4 10a4 10 0 0 0 4 -10a4 10 0 0 0 -4 -10" transform="rotate(45 12 12)" />
                    <path d="M12 2a4 10 0 0 0 -4 10a4 10 0 0 0 4 10a4 10 0 0 0 4 -10a4 10 0 0 0 -4 -10" transform="rotate(-45 12 12)" />
                  </svg>
                <h4>MATERIALES Y MAQUINARIAS</h4>
            </div>
            <p>Proveemos máquinas y productos de primera calidad.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-settings" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M10.325 4.317c.426 -1.756 2.924 -1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543 -.94 3.31 .826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756 .426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543 -.826 3.31 -2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756 -2.924 1.756 -3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543 .94 -3.31 -.826 -2.37 -2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756 -.426 -1.756 -2.924 0 -3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94 -1.543 .826 -3.31 2.37 -2.37c1 .608 2.296 .07 2.572 -1.065z" />
                    <circle cx="12" cy="12" r="3" />
                  </svg>
                <h4>SUPERVISION</h4>
            </div>
            <p>Ofrecemos supervisiones periódicas a nuestro personal.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-user-check" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <circle cx="9" cy="7" r="4" />
                    <path d="M3 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                    <path d="M16 11l2 2l4 -4" />
                  </svg>
                <h4>PERSONAL A CARGO</h4>
            </div>
            <p>Proveemos personal capacitado totalmente a nuestro cargo.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-gavel" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M13 10l7.383 7.418c.823 .82 .823 2.148 0 2.967a2.11 2.11 0 0 1 -2.976 0l-7.407 -7.385" />
                    <path d="M6 9l4 4" />
                    <path d="M13 10l-4 -4" />
                    <path d="M3 21h7" />
                    <path d="M6.793 15.793l-3.586 -3.586a1 1 0 0 1 0 -1.414l2.293 -2.293l.5 .5l3 -3l-.5 -.5l2.293 -2.293a1 1 0 0 1 1.414 0l3.586 3.586a1 1 0 0 1 0 1.414l-2.293 2.293l-.5 -.5l-3 3l.5 .5l-2.293 2.293a1 1 0 0 1 -1.414 0z" />
                  </svg>
                <h4>DAñOS Y PERJUICIOS</h4>
            </div>
            <p>Nos hacemos cargo por eventuales daños ocasionados.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-clock" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <circle cx="12" cy="12" r="9" />
                    <polyline points="12 7 12 12 15 15" />
                  </svg>
                <h4>HORARIOS CONVENIENTES</h4>
            </div>
            <p>Coordinados evitando entorpecer las tareas del cliente.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-camera-selfie" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M5 7h1a2 2 0 0 0 2 -2a1 1 0 0 1 1 -1h6a1 1 0 0 1 1 1a2 2 0 0 0 2 2h1a2 2 0 0 1 2 2v9a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-9a2 2 0 0 1 2 -2" />
                    <path d="M9.5 15a3.5 3.5 0 0 0 5 0" />
                    <line x1="15" y1="11" x2="15.01" y2="11" />
                    <line x1="9" y1="11" x2="9.01" y2="11" />
                  </svg>
                <h4>BUENA PRESENCIA</h4>
            </div>
            <p>Proveemos operarios uniformados acorde a las tareas a realizar.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-users" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <circle cx="9" cy="7" r="4" />
                    <path d="M3 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                    <path d="M16 3.13a4 4 0 0 1 0 7.75" />
                    <path d="M21 21v-2a4 4 0 0 0 -3 -3.85" />
                  </svg>
                <h4>RELEVO DE PERSONAL</h4>
            </div>
            <p>Posibilidad de solicitar cambio de empleados en caso necesario.</p>
        </article>
        <article class="item">
            <div class="logo">
                <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-plant" width="92" height="92" viewBox="0 0 24 24" stroke-width="1.5" stroke="#5772ff" fill="none" stroke-linecap="round" stroke-linejoin="round">
                    <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
                    <path d="M7 15h10v4a2 2 0 0 1 -2 2h-6a2 2 0 0 1 -2 -2v-4z" />
                    <path d="M12 9a6 6 0 0 0 -6 -6h-3v2a6 6 0 0 0 6 6h3" />
                    <path d="M12 11a6 6 0 0 1 6 -6h3v1a6 6 0 0 1 -6 6h-3" />
                    <line x1="12" y1="15" x2="12" y2="9" />
                  </svg>
                <h4>CUIDADO AMBIENTAL</h4>
            </div>
            <p>Cuidamos el medioambiente con productos de primera calidad.</p>
        </article>
    </section>
    {/if}
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
        flex-wrap: wrap;
        justify-content: space-evenly;
        align-items: center;
        gap: 1rem;
        padding: 1rem 0;
    }

    .item {
        text-align: center;
        width:20%;
        cursor:pointer;
        border-radius: 1rem;
        transition: all .2s ease;
        padding:1rem 0;
        border:2px solid transparent;

    }

    .item:hover {
        background: var(--secondary);
        border-left:2px groove var(--primary);
        border-right: 2px groove var(--primary);
    }

    h4 {
        text-transform: uppercase;
    }

    p {
        max-width:70%;
        margin:auto;
    }

    @media screen and (max-width:1200px) {
        #responsabilities {
            height:auto;
            padding:3vh 0 10vh;
            background-position: right center;
        }

        .container {
            min-width:75vw;
            height:auto;
            flex-wrap: wrap;
            align-items: center;
            justify-content: unset;
            flex-direction: column;
            border-radius: 1rem;
            background: none;
            box-shadow: none;
        }

        .item {
            width:auto;
            background:#fff;
            padding:1rem 0;
            border-radius: .5rem;
            border:1px solid var(--primary);
        }

        p {
            max-width:90%;
            margin:auto;
        }
    }
</style>