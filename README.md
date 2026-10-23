# HardTech Solutions — Site do grupo

Site institucional do grupo **HardTech Solutions** e das suas quatro unidades de negócio (BUs).
Tudo em **HTML, CSS e JavaScript estáticos** (sem framework, sem build): basta servir os arquivos.

> **Visão ampla. Precisão de lince.**

---

## Estrutura

```
HardTech/
├─ index.html            → HardTech Solutions (hub / marca-mãe do grupo)
├─ computers/index.html  → HardTech Computers  (assistência, montagem, upgrade)
├─ development/index.html→ HardTech Development (software sob medida)
├─ security/index.html   → HardTech Security   (consultoria em segurança)
├─ academy/index.html    → HardTech Academy    (cursos e treinamentos)
├─ assets/               → imagens compartilhadas (lince, emblema, sprites da corrida)
├─ robots.txt            → em computers/
└─ _previews/            → rascunhos e geração de imagens (NÃO vai para produção)
```

Cada pasta de BU tem cópias locais dos seus próprios arquivos (`favicon.png`, `hero-bg.jpg`,
`mountain-lynx.png`, etc.), para funcionar de forma independente.

---

## Identidade visual

- **Logo:** `HARD` + emblema (o "A" é a montanha com o lince no topo) + `TECH`.
- **Lince tribal** (`assets/lynx-tribal.png`): marca do grupo, usado na Solutions e na Security.
- **Montanha + lince** (`assets/mountain-lynx-v4.png`): emblema do "A" do logo e marca d'água de fundo.
- **Corrida do lince** (`assets/cycle-00..23.png`): 24 quadros usados na animação da Solutions.
- **Tipografia:** Orbitron (HARDTECH), Audiowide (SOLUTIONS/títulos), Chakra Petch (apoio), Michroma (BUs), Inter (texto das BUs).

### Cores por unidade
| Unidade      | Paleta (gradiente tri-tom)          |
|--------------|-------------------------------------|
| Computers    | roxo `#7C3AED` → `#9D4EDD` → `#3B82F6` |
| Development  | ciano `#0EA5E9` → `#22D3EE` → `#2DD4BF` |
| Security     | dourado `#D4A843` → `#F0B429` → `#F97316` |
| Academy      | rosa `#DB2777` → `#EC4899` → `#A855F7` |

---

## Composição de cada página

**Solutions (`index.html`)** — hub institucional para parceiros/investidores:
hero com animação (logo montado + roleta das BUs + lince correndo), apresentação do grupo
com marca d'água do emblema, ecossistema, unidades, diferenciais, missão/visão/valores,
governança e contato institucional (apenas e-mail).

**BUs** — cada landing tem: hero (slogan no centro, descritivo no canto, badge),
seções de serviço próprias de cada unidade, FAQ, formulário e contato via **WhatsApp**.
Cada BU tem uma animação temática própria (grade neon, código digitando, radar do lince,
partículas, trilha, etc.).

---

## Convenções

- **Contato:** a Solutions usa só **e-mail institucional**; as BUs usam **WhatsApp** (serviço).
- **Cache busting:** imagens atualizadas recebem `?v=N` na referência para forçar recarga.
- **Acessibilidade:** animações respeitam `prefers-reduced-motion`.

---

## Rodar localmente

É estático. Basta abrir `index.html` no navegador, ou servir a pasta:

```bash
# exemplo com Python
python -m http.server 8080
# depois acesse http://localhost:8080
```

## Deploy

O site é publicado via Cloudflare a partir da branch `main` deste repositório.
Por ser estático, o deploy não exige build — os arquivos são servidos como estão.
