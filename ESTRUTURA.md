# HardTech Solutions — Estrutura do projeto

Site do grupo **HardTech Solutions** (hub) com as 4 marcas (BUs). Pensado para publicar
como um único domínio: `hardtechsolutions.com/` (hub) + `/computers`, `/development`, etc.

## Pastas

```
HardTech/
├── index.html          ← HUB SOLUTIONS (home do domínio) — animação do logo + navegação
├── assets/             ← sprites do lince (cycle-00..23.png) + face-shadow.png
│
├── computers/          ← HardTech Computers  (tema roxo→azul→rosa)
│   └── index.html + logo.png, hero-bg.jpg, favicon.png, iconhardtechcomputers.jpeg, robots.txt
├── development/        ← HardTech Development (tema ciano→azul→turquesa)
│   └── index.html + assets visuais
├── security/           ← HardTech Security   (tema dourado→âmbar→laranja)
│   └── index.html + assets visuais
├── academy/            ← HardTech Academy    (tema rosa→magenta→roxo)
│   └── index.html + assets visuais
│
├── _previews/          ← Rascunhos e experimentos (NÃO faz parte do site)
└── ESTRUTURA.md
```

## Navegação (hub)

- A **home** (`index.html`) mostra a animação do logo Solutions e, na base, um menu fixo
  com as 4 BUs (cada botão na sua cor-tema). Clicar leva para `computers/`, `development/`, etc.
- Cada **BU** tem no header um link "← Solutions" que volta para a home (`../index.html`).

## Paletas tri-tom (estilo rico, como a Computers)

Cada BU usa 3 variáveis CSS `--p / --p2 / --az` que formam um gradiente vibrante:

| BU          | --p       | --p2      | --az      |
|-------------|-----------|-----------|-----------|
| Computers   | #7C3AED   | #9D4EDD   | #3B82F6   |
| Development | #0EA5E9   | #22D3EE   | #2DD4BF   |
| Security    | #D4A843   | #F0B429   | #F97316   |
| Academy     | #DB2777   | #EC4899   | #A855F7   |

## Observações

- WhatsApp do grupo em todas: 5515996880350.
- Analytics do Cloudflare só na página publicada original (agora removido das novas; reavaliar ao publicar o hub).
- Sprites do lince e rostos vieram de imagens com marca d'água (uso em preview). Para publicação
  oficial, substituir por arte licenciada ou própria.
- A animação da Solutions puxa as empresas do array `groups` no `<script>` do index.html raiz.

## Fontes
- **Orbitron** — HARDTECH / Michroma na Computers (logo original)
- **Audiowide** — SOLUTIONS
- **Chakra Petch** — taglines
