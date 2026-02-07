<!doctype html>
<html lang="cs">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Cyber doba</title>
        <link rel="preconnect" href="https://fonts.googleapis.com" />
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
        <link href="https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap" rel="stylesheet" />
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" />
        <style>
            body {
                /* pouzil jsem macos color picker pro presne barvicky */
                background-color: #0c1117;
                color: #fff;
                font-family: "Inter", sans-serif;
            }
            .logo-text {
                font-size: 32px;
                font-weight: 600;
                color: #59a6ff;
            }
            nav {
                display: flex;
                flex-direction: row;
                justify-content: space-between;
                align-items: center;
                background-color: #161b22;
                height: 7vh;
                border-bottom: 1px solid #30363d;
            }
            .logo {
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                gap: 10px;
                margin-left: 20vw;
            }
            .logo-image {
                width: 70px;
                height: 70px;
            }
            .nav-links {
                display: flex;
                flex-direction: row;
                justify-content: center;
                align-items: center;
                gap: 20px;
                color: gray;
                margin-right: 20vw;
                font-size: 14px;
            }
            a {
                color: gray;
                text-decoration: none;
            }
            .pripojit-se-button {
                background-color: #238636;
                color: #fff;
                padding: 10px 20px;
                border: none;
            }
            .horni-veci {
                display: flex;
                flex-direction: row;
            }
            .preziti {
                background-color: #23272f;
                color: lightgray;
                width: 15vw;
                justify-content: center;
                text-align: center;
            }
            .kyberzbrane {
                background-color: #2c3139;
                color: lightgray;
                width: 15vw;
                justify-content: center;
                text-align: center;
            }
            .sitovevalky {
                background-color: #353b44;
                color: lightgray;
                width: 15vw;
                justify-content: center;
                text-align: center;
            }
            .digitalniutiopie {
                background-color: #3b434b;
                color: lightgray;
                width: 15vw;
                justify-content: center;
                text-align: center;
            }
            .cyberdoba-image {
                width: 100%;
            }
            .img-footer {
                text-align: right;
                align-items: right;
                font-size: 12px;
                color: gray;
                background-color: #161b22;
                padding: 1px 15px;
            }
            main {
                margin-left: 20vw;
                margin-right: 20vw;
            }
            footer {
                display: flex;
                flex-direction: row;
                background-color: #0d1118;
                margin-left: 20vw;
                margin-right: 20vw;
                justify-content: space-between;
                align-items: flex-start;
                gap: 9vw;
                padding-left: 5vw;
                padding-right: 5vw;
                padding-top: 40px;
                padding-bottom: 40px;
            }
            .footer-onas {
                display: flex;
                flex-direction: column;
                justify-content: flex-start;
                align-items: flex-start;
                flex: 1;
            }
            .footer-onas h2 {
                font-size: 1rem;
                font-weight: bold;
                color: white;
                margin-bottom: 10px;
                margin-top: 0;
            }
            .footer-onas p {
                font-size: 0.9rem;
                color: gray;
                margin-bottom: 0px;
                margin-top: 0;
                line-height: 1.5;
            }
            .footer-kontakt {
                display: flex;
                flex-direction: column;
                justify-content: flex-start;
                align-items: flex-start;
                flex: 1;
            }
            .footer-kontakt h2 {
                font-size: 1rem;
                font-weight: bold;
                color: white;
                margin-bottom: 10px;
                margin-top: 0;
            }
            .footer-kontakt p {
                font-size: 0.9rem;
                color: gray;
                margin-bottom: 5px;
                margin-top: 0;
            }
            .footer-info {
                display: flex;
                flex-direction: column;
                justify-content: flex-start;
                align-items: flex-start;
                flex: 1;
                font-size: 0.9rem;
                color: gray;
            }
            .footer-info h2 {
                font-size: 1rem;
                font-weight: bold;
                color: white;
                margin-bottom: 10px;
                margin-top: 0;
            }
            .footer-info-item {
                font-size: 0.9rem;
                color: lightblue;
                margin-bottom: 5px;
                margin-top: 0;
                font-weight: bold;
            }
            .footer-info p:last-child {
                margin-top: 10px;
                margin-bottom: 0;
            }
            .quote {
                display: flex;
                flex-direction: column;
                gap: 10px;
                background-color: #14181f;
            }
            .quote-text {
                font-size: 24px;
                font-weight: bold;
                color: #59a6ff;
                margin-bottom: 10px;
                margin-top: 3vh;
                justify-content: center;
                align-items: center;
                text-align: center;
            }
            .quote-author {
                font-size: 16px;
                color: gray;
                margin-bottom: 3vh;
                margin-top: 0;
                justify-content: end;
                align-items: end;
                text-align: right;
                margin-right: 13vw;
            }
            .digitalninoc {
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                text-align: center;
                color: gray;
                padding-left: 5vw;
                padding-right: 5vw;
                background-color: #14181f;
            }
            .digitalninoc h1 {
                color: #59a6ff;
                text-align: center;
                margin-bottom: 0;
            }
            .digitalninoc hr {
                width: 10vw;
                color: gray;
            }
            .feature-cards {
                display: flex;
                flex-direction: row;
                justify-content: space-between;
                gap: 10px;
                padding: 40px 0;
                background-color: #161b22;
                padding-left: 5vw;
                padding-right: 5vw;
            }
            .feature-card {
                display: flex;
                flex-direction: column;
                align-items: center;
                padding: 20px;
                border: 2px solid;
                flex: 1;
                aspect-ratio: 1;
                min-height: 0;
            }
            .feature-card.blue {
                border-color: #59a6ff;
            }
            .feature-card.green {
                border-color: #3fb950;
            }
            .feature-icon {
                width: 25px;
                height: 25px;
                min-width: 25px;
                min-height: 25px;
                border-radius: 50%;
                border: 2px solid;
                display: flex;
                align-items: center;
                justify-content: center;
                margin-bottom: 20px;
                font-size: 28px;
            }
            .feature-card.blue .feature-icon {
                border-color: #59a6ff;
                color: #59a6ff;
            }
            .feature-card.green .feature-icon {
                border-color: #3fb950;
                color: #3fb950;
            }
            .feature-title {
                font-size: 1.2rem;
                font-weight: bold;
                margin-bottom: 15px;
                margin-top: 0;
                text-align: center;
            }
            .feature-card.blue .feature-title {
                color: #59a6ff;
            }
            .feature-card.green .feature-title {
                color: #3fb950;
            }
            .feature-description {
                font-size: 0.95rem;
                line-height: 1.4;
                margin: 0;
                text-align: center;
            }
            .feature-card.blue .feature-description {
                color: #59a6ff;
            }
            .feature-card.green .feature-description {
                color: #3fb950;
            }

            @media (max-width: 1000px) {
                .logo {
                    margin-left: 5vw;
                }
                .nav-links {
                    margin-right: 5vw;
                    gap: 15px;
                    font-size: 13px;
                }
                main {
                    margin-left: 5vw;
                    margin-right: 5vw;
                }
                footer {
                    margin-left: 5vw;
                    margin-right: 5vw;
                }
                .feature-cards {
                    flex-wrap: wrap;
                }
                .feature-card {
                    flex: 1 1 calc(50% - 5px);
                    min-width: calc(50% - 5px);
                }
            }

            @media (max-width: 750px) {
                nav {
                    flex-wrap: wrap;
                    height: auto;
                    min-height: 7vh;
                    padding: 10px 0;
                }
                .logo {
                    margin-left: 5vw;
                    width: 100%;
                    justify-content: flex-start;
                }
                .logo-image {
                    width: 50px;
                    height: 50px;
                }
                .logo-text {
                    font-size: 24px;
                }
                .nav-links {
                    margin-right: 5vw;
                    margin-left: 5vw;
                    width: calc(100% - 10vw);
                    flex-wrap: wrap;
                    gap: 10px;
                    margin-top: 10px;
                }
                .nav-links a {
                    font-size: 12px;
                }
                .pripojit-se-button {
                    padding: 8px 16px;
                    font-size: 12px;
                }
                .horni-veci {
                    flex-direction: column;
                }
                .preziti,
                .kyberzbrane,
                .sitovevalky,
                .digitalniutiopie {
                    width: 100%;
                    padding: 15px 0;
                }
                main {
                    margin-left: 0;
                    margin-right: 0;
                }
                .quote {
                    padding-left: 5vw;
                    padding-right: 5vw;
                }
                .quote-author {
                    margin-right: 0;
                }
                .img-footer {
                    padding-left: 5vw;
                    padding-right: 5vw;
                }
                .feature-cards {
                    flex-direction: column;
                    gap: 20px;
                    padding-left: 5vw;
                    padding-right: 5vw;
                }
                .feature-card {
                    width: 100%;
                    flex: 1 1 100%;
                    aspect-ratio: auto;
                    min-height: 220px;
                    max-width: 100%;
                }
                .feature-title {
                    font-size: 1.1rem;
                }
                .feature-description {
                    font-size: 0.9rem;
                    line-height: 1.5;
                }
                footer {
                    flex-direction: column;
                    margin-left: 5vw;
                    margin-right: 5vw;
                    gap: 30px;
                    padding-left: 0;
                    padding-right: 0;
                }
                .footer-onas,
                .footer-kontakt,
                .footer-info {
                    width: 100%;
                }
            }

            @media (max-width: 450px) {
                .logo {
                    margin-left: 3vw;
                }
                .logo-text {
                    font-size: 20px;
                }
                .logo-image {
                    width: 40px;
                    height: 40px;
                }
                .nav-links {
                    margin-left: 3vw;
                    margin-right: 3vw;
                    width: calc(100% - 6vw);
                    flex-direction: column;
                    align-items: flex-start;
                    gap: 8px;
                }
                .nav-links a {
                    font-size: 11px;
                }
                .pripojit-se-button {
                    width: 100%;
                    padding: 10px;
                }
                .quote-text {
                    font-size: 18px;
                    padding: 0 3vw;
                }
                .quote {
                    padding-left: 3vw;
                    padding-right: 3vw;
                }
                .quote-author {
                    margin-right: 0;
                    font-size: 14px;
                }
                .img-footer {
                    padding-left: 3vw;
                    padding-right: 3vw;
                }
                .digitalninoc {
                    padding-left: 3vw;
                    padding-right: 3vw;
                }
                .digitalninoc h1 {
                    font-size: 24px;
                }
                .feature-cards {
                    padding-left: 3vw;
                    padding-right: 3vw;
                    gap: 15px;
                }
                .feature-card {
                    min-height: 200px;
                    padding: 15px;
                }
                .feature-icon {
                    width: 20px;
                    height: 20px;
                    min-width: 20px;
                    min-height: 20px;
                    font-size: 24px;
                    margin-bottom: 15px;
                }
                .feature-title {
                    font-size: 1rem;
                    margin-bottom: 12px;
                }
                .feature-description {
                    font-size: 0.85rem;
                    line-height: 1.5;
                }
                footer {
                    margin-left: 3vw;
                    margin-right: 3vw;
                    padding-top: 30px;
                    padding-bottom: 30px;
                }
            }
        </style>
    </head>
    <body>
        <nav>
            <div class="logo">
                <img src="https://api.ssps.cajthaml.eu/file/69335fbb6945137e5671b038" alt="logo" class="logo-image" />
                <p class="logo-text">CyberCorp</p>
            </div>

            <div class="nav-links">
                <a href="#">Zpravy z podsveti</a>
                <a href="#">Kybernetika</a>
                <a href="#">Hackerska elita</a>
                <a href="#">Casto hackovane otazky</a>
                <button class="pripojit-se-button">PRIPOJIT SE</button>
            </div>
        </nav>
        <main>
            <section class="horni-veci">
                <div class="preziti">
                    <p>PREZITI</p>
                </div>
                <div class="kyberzbrane">
                    <p>KYBERZBRANE</p>
                </div>
                <div class="sitovevalky">
                    <p>SITOVE VALKY</p>
                </div>
                <div class="digitalniutiopie">
                    <p>DIGITALNI UTOPIE</p>
                </div>
            </section>
            <img src="https://api.ssps.cajthaml.eu/file/69335fb128ac5f259ab1763a" alt="cyberdoba" class="cyberdoba-image" />
            <aside class="img-footer">
                <p>2126 © CyberCorp - Vsechna prava zasifrovana</p>
                <!-- copyright symbol je proste option + G na macu takze jsem ho nikde nehledal -->
            </aside>
            <article class="digitalninoc">
                <h1>DIGITALNI NOC</h1>
                <hr />
                <p>
                    V roce 2162 se svet rozdelil na osvicene megamesta a ruzne tyhle veci, pisu tady nahodny text, jelikoz nechci porad vyuzivat lorem ipsum, ale vidim to tak, ze misto kopirovani lorem ipsum proste zacnu psat co si z nej pamatuji. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos. Vic si nepamatuji <br />
                    <br />
                    V roce 2162 se svet rozdelil na osvicene megamesta a ruzne tyhle veci, pisu tady nahodny text, jelikoz nechci porad vyuzivat lorem ipsum, ale vidim to tak, ze misto kopirovani lorem ipsum proste zacnu psat co si z nej pamatuji. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos. Vic si nepamatuji <br />
                    <br />
                    V roce 2162 se svet rozdelil na osvicene megamesta a ruzne tyhle veci, pisu tady nahodny text, jelikoz nechci porad vyuzivat lorem ipsum, ale vidim to tak, ze misto kopirovani lorem ipsum proste zacnu psat co si z nej pamatuji. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quos. Vic si nepamatuji <br />
                    <br />
                </p>
            </article>
            <section class="feature-cards">
                <div class="feature-card blue">
                    <div class="feature-icon">
                        <i class="fas fa-robot"></i>
                    </div>
                    <h3 class="feature-title">AI ROZVOJ</h3>
                    <p class="feature-description">Kyberumelci posouvaji hranice kreativity ve spojeni s umelou inteligenci.</p>
                </div>
                <div class="feature-card green">
                    <div class="feature-icon">
                        <i class="fas fa-key"></i>
                    </div>
                    <h3 class="feature-title">BEZPECNOST</h3>
                    <p class="feature-description">Data jsou menou. Vase soukromi? Iluze v rukou megakorporaci.</p>
                </div>
                <div class="feature-card blue">
                    <div class="feature-icon">
                        <i class="fas fa-vr-cardboard"></i>
                    </div>
                    <h3 class="feature-title">BUDOUCNOST</h3>
                    <p class="feature-description">Nova era zacina ve virtualnim svete - realita ztraci vyznam.</p>
                </div>
                <div class="feature-card green">
                    <div class="feature-icon">
                        <i class="fas fa-network-wired"></i>
                    </div>
                    <h3 class="feature-title">KYBERSITE</h3>
                    <p class="feature-description">Pripojte se. Budte soucasti boje za svobodu na darknetu.</p>
                </div>
            </section>
            <article class="quote">
                <p class="quote-text">“Vsechno je data. Nezalezi na tom, co je skutecne.”</p>
                <p class="quote-author">- CyberProphet</p>
            </article>
        </main>
        <footer>
            <div class="footer-onas">
                <h2>O nas</h2>
                <p>CyberCorp je nejvetsi sitova komunita, ktera propojuje mysl a budoucnost.</p>
            </div>
            <div class="footer-kontakt">
                <h2>Kontakt</h2>
                <p>info@cybercorp.net</p>
                <p>+420 284 016 666</p>
            </div>
            <div class="footer-info">
                <h2>Informace</h2>
                <p class="footer-info-item">PODPORA</p>
                <p class="footer-info-item">TECHNOLOGIE</p>
                <p class="footer-info-item">HACKERSKA AKADEMIE</p>
                <p>2126 © CyberCorp</p>
            </div>
        </footer>
    </body>
</html>
