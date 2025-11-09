# 🦷 Clínica Odontológica — Base para Responsividade

Landing page **estática (HTML + CSS)** usada **como base** para ensinar e demonstrar **responsividade** 📱.  
Sem frameworks, sem build, nem JS obrigatório (apenas um script simples no rodapé para o ano atual).

---

## ▶️ Como rodar (DEV)

1. Tenha um navegador instalado (qualquer moderno serve).
2. Na pasta do projeto, você pode:
   - Abrir **`index.html`** direto no navegador, **ou**
   - Servir localmente:
     - `npx serve .`  
     - **ou** `python -m http.server`  
     - **ou** `php -S localhost:3000 -t .`  
3. Acesse: `http://localhost:3000` (caso use servidor).

> 💡 Dica: manter a estrutura de pastas como está para evitar erros de caminho nas imagens.

---

## 🗂️ Estrutura de Pastas (sugerida)

```
clinica-responsiva/
├─ index.html
├─ style.css
└─ imagens/
   ├─ logo.png
   ├─ equipe-hero.png
   ├─ equipe-sobre.png
   ├─ icones/
   │  ├─ clareamento.png
   │  ├─ implantes.png
   │  ├─ ortodontia.png
   │  └─ limpeza.png
   └─ pacientes/
      ├─ p1.jpg
      ├─ p2.jpg
      └─ p3.jpg
```

---

## 🧩 O que esta base oferece

- **HTML semântico**: `header`, `main`, `section`, `footer`.
- **Seções**: Header, Hero, Serviços, Sobre, Depoimentos, Localização, CTA, Rodapé.
- **Ícones e imagens fictícias** organizadas por pasta.
- **CSS com Nesting** (CSS nativo): organizado por bloco/seção.
- **Âncoras** e `scroll-behavior: smooth;`.

> 💡 Observação: O CSS utiliza **CSS Nesting nativo**, já suportado nos browsers modernos. Não há preprocessadores.

---

## 📏 Onde mexer para ensinar responsividade

- **Container**: largura fluida com `max-width` em `style.css`.
- **Hero (grid/flex)**: empilhar no mobile e lado a lado a partir de `768px+`.
- **Serviços (grid)**: 1 → 2 → 3 → 4 colunas conforme breakpoints.
- **Depoimentos (flex)**: coluna no mobile, wrap no tablet/desktop.
- **Localização (duas colunas)**: empilhado no mobile, lado a lado em telas médias+.
- **Tipografia fluida**: use `clamp()` nos títulos (ex.: `clamp(28px, 5vw, 48px)`).
- **Imagens elásticas**: `max-width: 100%; height: auto;`.

---

## 🧭 Navegação & Acessibilidade

- Links do menu apontam para seções com `id`.
- Imagens com `alt` descritivo (hero, equipe) e ícones decorativos podem usar `alt=""`.
- Seções “Sobre” e “Localização” podem usar `aria-labelledby` para o título da seção.

---

## 🧪 Teste rápido de responsividade

- DevTools → **Toggle device toolbar** (Ctrl/Cmd+Shift+M).
- Teste larguras populares: **360 / 390 / 768 / 992 / 1200+**.
- Observe: grid de serviços, empilhamento de hero/sobre/localização e legibilidade de textos.

---

## 🔒 Escopo

- **Foco**: HTML + CSS desta própria landing page como **base** de aula.
- Ajustes são feitos **diretamente em `style.css`** ao vivo.

---

## 📄 Licença & Imagens

- Uso **educacional** e de **demonstração**.
- Imagens/nomes **fictícios** (placeholders).
