# Guilherme Santini — Portfolio

Portfolio pessoal em formato de álbum de figurinhas, apresentando projetos web e mobile desenvolvidos com PWA, Firebase, Angular e JavaScript.

🔗 **Live:** [guilhermesantinidev.github.io](https://guilhermesantinidev.github.io)

## ✨ Sobre

Página única (`index.html`) com visual de álbum de figurinhas colecionáveis: cada projeto é uma "figurinha" que pode ser marcada como vista, com persistência local via `localStorage`. Projetos com case study detalhado têm um link extra para uma página dedicada em `/cases`.

## 📁 Estrutura

```
.
├── index.html              # Página principal do portfolio
└── cases/                  # Case studies individuais
    └── biblical-verse.html # Case study: My Biblical Verse
```

Cada novo case study segue o padrão `cases/nome-do-projeto.html` e é referenciado no sticker correspondente em `index.html` através do link "Ver case study".

## 🛠️ Stack

- HTML, CSS e JavaScript puro (sem build step, sem dependências)
- Google Fonts (Space Grotesk, Caveat, Inter, Space Mono)
- `localStorage` para persistir progresso da coleção
- `IntersectionObserver` para animações de entrada

## 🚀 Publicando no GitHub Pages

1. Suba este repositório para o GitHub (ex: `guilhermesantinidev/guilhermesantinidev.github.io` para domínio raiz, ou qualquer outro nome de repo).
2. Vá em **Settings → Pages**.
3. Em **Source**, selecione a branch `main` e a pasta `/ (root)`.
4. Salve. O site fica disponível em poucos minutos em `https://<usuario>.github.io/<repo>/` (ou na raiz, se o repo for `<usuario>.github.io`).

Não há processo de build — os arquivos são servidos como estão.

## ➕ Adicionando um novo projeto

1. Crie o case study em `cases/nome-do-projeto.html` (pode copiar a estrutura de `cases/biblical-verse.html` como ponto de partida).
2. No `index.html`, adicione o link "Ver case study" no sticker do projeto correspondente, dentro de `.sticker-links`.
3. Garanta que o link "← Voltar ao portfolio" do novo case study apontap para `../index.html`.

## 📄 Licença

Projeto pessoal de portfolio. Sinta-se livre para usar a estrutura como referência.
