<script>
    import { fly } from 'svelte/transition'

    let y
</script>

<svelte:window bind:scrollY={y}/>

<section id="materials">
    {#if y >= 1372}
    <article class="modal" transition:fly="{{ y: -100, duration: 1200 }}">
        <h3>Materiales</h3>
        <p>Todos nuestro productos respetan el medio ambiente ya que son de primera marca, no tóxicos, no corrosivos y biodegradables.

            Pese a la diversidad y especialización de los materiales con los que contamos mantenemos una inmensa responsabilidad con el medio ambiente por lo que operamos única y exclusivamente con productos no contaminables.</p>
    </article>
    <article class="modal" transition:fly="{{ y: -100, duration: 1200 }}">
        <h3>Maquinaria</h3>
        <p>Full Wipe se encarga de proveer las máquinas que sean necesarios para realizar la prestación del servicio. Por razones operativas, deben quedar de modo permanente en el lugar de trabajo. Por este motivo, es importante que el cliente disponga de un lugar destinado a guardar las herramientas de limpieza.</p>
    </article>
    {/if}
</section>

<style>
    #materials {
        height:105vh;
        width:100vw;
        background: url('/materials_bg.png') no-repeat top center;
        border-top: 2px solid var(--primary);
        border-bottom: 5px solid var(--primary);
        display:flex;
        align-items: center;
        justify-content: space-evenly;
    }

    .modal {
        width:30%;
        height:40%;
        background: var(--secondary);
        color: #f5f5f5;
        font-weight: 500;
        display:flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: center;
        padding: 4rem;
        border-radius: 1rem;
        border:2px solid var(--primary);
    }

    h3 {
        font-size:2rem;
    }

    p {
        font-size:1.25rem;
    }

    @media screen and (max-width: 1200px) {
        #materials {
            height:90vh;
            width:auto;
            padding:5vh 0;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .modal {
            width:auto;
            height:auto;
            padding: 2rem;
            margin:2rem;
        }

        h3 {
            font-size:1.5rem;
        }

        p {
            font-size:1rem;
        }
    }
</style>