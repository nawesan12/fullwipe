<section id="contact">
    <section class="logo-and-social">
        <img src="/images/wipe.png" alt="Logo">
        <ul class="social-list">
            <li><a href="callto:+542235929292"><span>Whatsapp:</span> 223 5 929292</a></li>
            <li><a href="https://facebook.com"><span>Facebook:</span> Full Wipe</a></li>
            <li><a href="mailto:fullwipe@gmail.com"><span>Email:</span> fullwipe@gmail.com</a></li>
        </ul>
    </section>
    <section class="form-grid">
        <input type="text" class="name" placeholder="Nombre"/>
        <input type="text" class="email" placeholder="Email"/>
        <input type="text" class="phone" placeholder="Telefono"/>
        <textarea placeholder="Mensaje"></textarea>
    </section>
    <button class="submit_button">Enviar</button>
</section>

<style>
    #contact {
        background: url('/contact_bg.svg') no-repeat center center;
        height:100vh;
        max-width:100vw;
        display:flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-evenly;
    }

    textarea {
        resize:none;
    }

    .logo-and-social {
        width:60vw;
        display:flex;
        align-items: center;
        justify-content: space-around;
    }

    img {
        height:20rem;
    }

    ul {
        list-style: none;
        display:flex;
        flex-direction: column;
        justify-content: space-around;
    }

    li {
        font-size: 1.2rem;
        margin:0.5rem;
    }

    span {
        font-weight: 500;
    }

    .form-grid {
        display:grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 3rem 1fr;
        grid-gap: 1rem;
        width:60vw;
        height:30vh;
    }

    input {
        padding: 0 1rem;
        border: none;
        border-bottom: 1px solid #ccc;
        outline:none;
        font-size:1.1rem;
        border-radius: .7rem;
    }

    textarea {
        grid-row: 2 / 3;
        grid-column: 1 / 4;
        padding: 1rem;
        border: none;
        border-bottom: 1px solid #ccc;
        outline:none;
        font-size:1.1rem;
        border-radius: .7rem;
    }

    .name {
        grid-row: 1 / 2;
        grid-column: 1 / 2;
    }

    .email {
        grid-row: 1 / 2;
        grid-column: 2 / 3;
    }

    .phone {
        grid-row: 1 / 2;
        grid-column: 3 / 4;
    }

    .submit_button {
        padding:1rem 2rem;
        border:none;
        border-radius: .7rem;
        background: none;
        font-size:1.1rem;
        font-weight: 500;
        cursor: pointer;
        color:#f5f5f5;
        border: 2px solid #f5f5f5;
    }

    @media screen and (max-width:1200px) {
        #contact {
            height:auto;
            max-width:100vw;
            display:flex;
            flex-direction: column;
            align-items: center;
        }

        .logo-and-social {
            width:100vw;
            display:flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 5vh;
        }

        img {
            height:18rem;
        }

        ul {
            list-style: none;
            display:flex;
            flex-direction: column;
            justify-content: space-around;
        }

        li {
            font-size: 1.5rem;
            margin:0.5rem;
        }

        .form-grid {
            display:flex;
            flex-direction: column;
            width:100vw;
            height:auto;
        }

        input, textarea {
            padding:1rem;
            display:block;
            margin: auto;
            width:80vw;
        }

        textarea {
            padding: 1rem;
            border: none;
            border-bottom: 1px solid #ccc;
            outline:none;
            font-size:1.1rem;
            border-radius: .7rem;
            height:10rem;
        }

        .submit_button {
            margin: 5vh 0;
        }
    }
</style>