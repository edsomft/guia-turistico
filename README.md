# Guia Turístico — Vale do Jaguaribe

Projeto desenvolvido para a disciplina de Desenvolvimento Web (Prof. Silas Santiago), do curso Técnico/Superior em Dev Web — IFCE Campus Aracati.

**Integrante:** Edsom Fontes ([@edsomft](https://github.com/edsomft))

## Descrição do projeto

Site estático com foco em HTML semântico, apresentando um guia de pontos turísticos da região do Vale do Jaguaribe (CE). O projeto conta com três páginas:

- **index.html** — Página inicial com 10 pontos turísticos, cada um com imagem, descrição e mapa de localização.
- **about.html** — Informações sobre o desenvolvedor e as tecnologias utilizadas.
- **contact.html** — Formulário de inscrição para passeios turísticos na região.

O projeto foi criado com **Vite + Vanilla JS**, utilizado apenas como ferramenta de build e servidor de desenvolvimento — o conteúdo das páginas não depende de JavaScript.

## Como rodar o projeto localmente

Pré-requisitos: [Node.js](https://nodejs.org) instalado.

```bash
# clonar o repositório
git clone https://github.com/edsomft/guia-turistico.git
cd guia-turistico

# instalar as dependências
npm install

# rodar o servidor de desenvolvimento
npm run dev
```

O projeto abrirá em `http://localhost:5173`. As páginas podem ser acessadas em:
- `/index.html`
- `/about.html`
- `/contact.html`

## Site publicado

🔗 [https://edsomft.github.io/guia-turistico/](https://edsomft.github.io/guia-turistico/)

## Checklist de recursos HTML implementados

| Recurso | Onde foi usado |
|---|---|
| Estrutura semântica (`header`, `nav`, `main`, `section`, `article`, `aside`, `footer`) | `index.html`, `about.html`, `contact.html` |
| `<meta name="viewport">` | `index.html`, `about.html`, `contact.html` |
| `<meta name="description">` | `index.html`, `about.html`, `contact.html` |
| `<link rel="icon">` (favicon customizado) | `index.html`, `about.html`, `contact.html` |
| `<picture>` / `<source>` / `<img>` (imagens responsivas) | `index.html` (10 pontos turísticos) |
| `<iframe>` (mapas do Google Maps) | `index.html` |
| `<video>` / `<track>` | `index.html` |
| `<details>` / `<summary>` | `index.html` |
| `<dialog>` | `index.html` |
| Formatação textual (`strong`, `em`, `mark`, `small`, `del`, `ins`, `sub`, `sup`) | `about.html` |
| `<table>` | `about.html` |
| `<ul>` / `<li>` | `about.html` |
| Formulário completo (`email`, `tel` com `pattern`, `date`, `number`, `range`, `radio`, `checkbox`) | `contact.html` |
| `accesskey` | `index.html`, `about.html`, `contact.html` (menu de navegação) |
| `contenteditable` | `about.html` |
| `download` | `contact.html` |
| `loading="lazy"` | `index.html` |
| `alt` descritivo | `index.html` |
| `aria-label` | `index.html` (mapas) |


## Diário de Desenvolvimento (DevLog)

### Dia 1 — 03/08/2026
- Criação do repositório no GitHub e adição do professor como colaborador.
- Configuração inicial do projeto com Vite (Vanilla JS).

### Dia 2 — 04/08/2026
- Configuração do `vite.config.js` para build multi-página (index, about, contact).
- Criação do esqueleto das páginas `about.html` e `contact.html`.

### Dia 3 — 06/08/2026
- Implementação da estrutura semântica da página inicial (header, nav, main, section, footer).
- Criação do primeiro ponto turístico como modelo (Praia de Redonda), com imagem responsiva, descrição em `<details>` e mapa via `<iframe>`.
- Replicação do padrão para os demais 9 pontos turísticos.
