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

