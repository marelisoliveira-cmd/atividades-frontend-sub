# Professor-Gabriel-
Frond-and

Código 1
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 
    <title>Meu primeiro projeto Front-End</title> 
    <link rel="stylesheet" href="estilo.css"> 
    <script src="script.js" defer></script>
</head>
<body>
    <header class="cabecalho">
        <p class="etiqueta">Programação Front-End • 2º DS Subsequente</p>
        <h1>Meu primeiro projeto Front-End</h1>
        <p>Uma página organizada para conferir se HTML, CSS e JavaScript estão conectados corretamente.</p>
    </header>

    <main>
        <section class="painel" aria-labelledby="titulo-arquivos">
            <h2 id="titulo-arquivos">Arquivos do projeto</h2>
            <div class="grade-arquivos">
                <article>
                   <strong>index.html</strong>
                   <span>Organiza o conteúdo e conecta os demais arquivos.</span>
                </article>
                <article>
                    <strong>estilo.css</strong>
                    <span>Controla cores, espaçamentos e responsividade.</span>
                </article>
                <article>
                    <strong>script.js</strong>
                    <span>Adiciona comportamento e responde às ações do usuário.</span>
                </article>
                <article>
                    <strong>README.md</strong>
                    <span>Documenta o projeto, o estudante e a forma de execução.</span>
                </article>
            </div>
        </section>
        
        <section class="painel" aria-labelledby="titulo-teste">
            <h2 id="titulo-teste">Teste do ambiente</h2>
            <p>Abra a página no navegador e use o botão para verificar a ligação entre os arquivos.</p>
            <button id="testarProjeto" type="button">Verificar projeto</button>
            <p id="statusProjeto" class="status" aria-live="polite">Aguardando a verificação.</p>
        </section>
    </main>

    <footer>
        <p>Exercício FE01 • Colégio Estadual Alberto Gomes Veiga</p>
    </footer>
</body>
</html>



Segundo código 

:root {
--fundo: #07111f;
--painel: #10243a;
--painel-claro: #173653;
--texto: #f3f7ff;
--texto-suave: #b8c7da;
--destaque: #38bdf8;
--sucesso: #4ade80;
--borda: #2b4d6c;
}

* {
    box-sizing: border-box;
}

body {
    margin: 0; 
    min-height: 100vh;
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(145deg, #050b14, var(--fundo));
    color: var(--texto);
}

.cabecalho,
main, 
footer {
    width: min(960px, 92%); 
    margin-inline: auto;
}

.cabecalho {
    padding: 48px 0 24px;
}

.etiqueta {
    color: var(--destaque);
    font-weight: 700;
    letter-spacing: 0.04em;
}

h1,
h2,
p {
    margin-top: 0;
}

h1 {
    font-size: clamp(2rem, 5vw, 3.7rem);
    margin-bottom: 12px;
}

p,
span {
    color: var(--texto-suave);
    line-height: 1.6;
}

.painel {
    padding: 24px;
    margin-bottom: 20px;
    background: rgba(16, 36, 58, 0.92);
    border: 1px solid var(--borda);
    border-radius: 18px;
}

.grade-arquivos {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 14px;
}

article {
    display: grid;
    gap: 8px;
    padding: 18px;
    background: var(--painel-claro);
    border: 1px solid var(--borda);
    border-radius: 14px;
}

button {    
    min-height: 48px;
    padding: 12px 18px;
    border: 0; 
    border-radius: 12px;
    background: var(--destaque);
    color: #04131f;
    font: inherit;
    font-weight: 800;
    cursor: pointer;
}

    button:hover,
    button:focus-visible {
        filter: brightness(1.1);
}

    .status {
        margin-top: 16px;
        padding: 14px;
        background: #07192a;
        border-left: 4px solid var(--destaque);
        border-radius: 8px;
}

    .status.sucesso {
        color: var(--sucesso);
        border-left-color: var(--sucesso);
}

    footer {
        padding: 8px 0 36px;
}

@media (max-width: 640px) {
    .cabecalho {
        padding-top: 28px;
    }

    .painel {
        padding: 18px;
}

.grade-arquivos {
    grid-template-columns: 1fr;
}

    button {
        width: 100%;
    }
}

Código 3

const botaoTeste = document.querySelector('#testarProjeto');
const statusProjeto = document.querySelector('#statusProjeto');

botaoTeste.addEventListener('click', () => {
    statusProjeto.textContent = 'Projeto verificado: HTML, CSS e JavaScript estão conectados.';
    statusProjeto.classList.add('sucesso');
    botaoTeste.textContent = 'Ambiente verificado';
});


Código 4 

# FE01 - Meu primeiro projeto Front-End

Primeiro projeto da disciplina **Programação Front-End**, organizado para testar a ligação entre HTML, CSS e JavaScript.

## Estrutura da pasta

```text
exercicio-01/
-  index.html
-  estilo.css
-  script.js
-  README.md
```

## Como executar

1. Abra a pasta no Visual Studio Code.
2. Abra o arquivo `index.html` no navegador ou utilize a extensão Live Server.
3. Clique em **Verificar projeto**.
4. Confirme se a mensagem de sucesso aparece na página.

## Identificação do estudante

- Nome: **substitua pelo seu nome**
- Turma: **2 DS Subsequente - Noturno**
- Forma escolhida para executar: **descreva aqui**

## Entrega

Envie o link do repositório solicitado pelo professor e anexe a evidência gerada pela plataforma.

Atividade 2

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horizonte Soluções Digitais</title>

    <link rel="stylesheet" href="estilo.css">
    <script src="script.js" defer></script>
</head>

<body>

    <a class="pular-conteudo" href="#conteudo">
        Pular para o conteúdo principal
    </a>

    <header class="cabecalho">
        <p class="etiqueta">Tecnologia para pequenos negócios</p>

        <h1>Horizonte Soluções Digitais</h1>

        <p>
            Organizamos presença digital, atendimento e processos para empresas
            que desejam crescer.
        </p>

        <nav aria-label="Navegação principal">
            <ul>
                <li><a href="#servicos">Serviços</a></li>
                <li><a href="#processo">Como trabalhamos</a></li>
                <li><a href="#equipe">Equipe</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <main id="conteudo">

        <section id="servicos" aria-labelledby="titulo-servicos">
            <h2 id="titulo-servicos">Serviços para a rotina da empresa</h2>

            <p>
                Cada serviço resolve uma necessidade comum de organização,
                divulgação ou relacionamento com clientes.
            </p>

            <article>
                <h3>Site institucional</h3>
                <p>
                    Página profissional para apresentar a empresa, seus serviços
                    e os canais de contato.
                </p>
            </article>

            <article>
                <h3>Catálogo digital</h3>
                <p>
                    Organização de produtos ou serviços em uma experiência
                    simples para computadores e celulares.
                </p>
            </article>

            <article>
                <h3>Automação de atendimento</h3>
                <p>
                    Formulários e fluxos básicos para reduzir tarefas repetitivas
                    e registrar solicitações.
                </p>
            </article>
        </section>

        <section id="processo" aria-labelledby="titulo-processo">
            <h2 id="titulo-processo">Como trabalhamos</h2>

            <ol>
                <li>Entendemos o problema e as pessoas envolvidas.</li>
                <li>Organizamos o conteúdo e desenhamos a solução.</li>
                <li>Construímos, testamos e registramos as melhorias.</li>
            </ol>
        </section>

        <section id="equipe" aria-labelledby="titulo-equipe">
            <h2 id="titulo-equipe">Equipe responsável</h2>

            <p>
                Profissionais de atendimento, design e desenvolvimento trabalham
                juntos para entregar soluções de qualidade.
            </p>
        </section>

        <aside id="atendimento" aria-labelledby="titulo-atendimento">
            <h2 id="titulo-atendimento">Atendimento</h2>

            <p>Precisa conversar antes de solicitar um projeto?</p>

            <button
                id="mostrarAtendimento"
                type="button"
                aria-expanded="false"
                aria-controls="detalhesAtendimento">
                Mostrar horários
            </button>

            <div id="detalhesAtendimento" hidden>
                <p>Segunda a sexta, das 8h às 18h.</p>
                <p>Retorno inicial em até um dia útil.</p>
            </div>
        </aside>

    </main>

    <footer id="contato">
        <h2>Contato profissional</h2>

        <address>
            Avenida Central, 250 - Curitiba/PR<br>
            <a href="mailto:contato@horizontedigital.example">
                contato@horizontedigital.example
            </a>
        </address>

        <p>Exercício FE02 - Programação Front-End</p>
    </footer>

</body>
</html>

Exercicio 2

segundo código 

:root {
    --fundo: #08121f;
    --superficie: #10243a;
    --superficie-clara: #183754;
    --texto: #f5f8ff;
    --texto-suave: #c2cede;
    --destaque: #67e8f9;
    --borda: #31516f;
    --sucesso: #86efac;
}

* {
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
    background: var(--fundo);
    color: var(--texto);
}

.pular-conteudo {
    position: absolute;
    left: 16px;
    top: -80px;
    padding: 12px 16px;
    background: var(--destaque);
    color: #04131f;
    font-weight: 700;
    border-radius: 8px;
}

.pular-conteudo:focus {
    top: 16px;
}

h2,
h3,
p {
    margin-top: 0;
}

header,
main,
footer {
    width: min(900px, 92%);
    margin-inline: auto;
}

header {
    padding: 52px 0 28px;
}

.etiqueta {
    color: var(--destaque);
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.08em;
}

h1 {
    max-width: 760px;
    margin: 0 0 12px;
    font-size: clamp(2.2rem, 7vw, 4.6rem);
    line-height: 1.1;
}

p,
li,
address {
    color: var(--texto-suave);
    line-height: 1.65;
}

nav {
    margin-top: 26px;
    padding-top: 18px;
    border-top: 1px solid var(--borda);
}

nav ul {
    margin: 0;
    padding: 0;
    list-style: none;
}

nav li {
    display: inline-block;
    margin: 0 18px 10px 0;
}

nav a {
    color: var(--destaque);
    font-weight: 700;
    text-decoration-thickness: 2px;
    text-underline-offset: 5px;
}

section,
aside,
footer {
    margin-bottom: 22px;
    padding: 24px;
    background: var(--superficie);
    border: 1px solid var(--borda);
    border-radius: 16px;
}

article {
    margin-top: 14px;
    padding: 18px;
    background: var(--superficie-clara);
    border-left: 4px solid var(--destaque);
    border-radius: 10px;
    padding-left: 24px;
}

button {
    min-height: 48px;
    padding: 12px 18px;
    border: 0;
    border-radius: 10px;
    background: var(--destaque);
    color: #04131f;
    font: inherit;
    font-weight: 800;
    cursor: pointer;
}

button:hover,
button:focus-visible {
    filter: brightness(1.08);
}

#detalhesAtendimento {
    margin-top: 18px;
    padding: 16px;
    border: 1px solid var(--sucesso);
    border-radius: 10px;
}

#detalhesAtendimento p:last-child {
    margin-bottom: 0;
}

footer {
    margin-bottom: 38px;
}

address {
    font-style: normal;
}

@media (max-width: 520px) {
    header {
        padding-top: 34px;
    }

    section,
    aside,
    footer {
        padding: 18px;
    }

    nav li {
        display: block;
        margin-right: 0;
    }

    button {
        width: 100%;
    }
}

