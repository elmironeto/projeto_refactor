# Situação de Aprendizagem: Auditoria e Refatoração de um Site Institucional

**Componente curricular:** Desenvolvimento Web (HTML e CSS)
**Duração sugerida:** 2 aulas

---

## 1. Cenário

A **ONG Instituto Vale Verde** contratou um freelancer para criar o site institucional às pressas. O resultado foi entregue, mas a diretoria percebeu vários problemas: o menu quebra em telas pequenas, o texto do rodapé é quase ilegível, o botão de contato não funciona com teclado, e o código, quando colado em um validador, acusa múltiplos erros.

Você foi contratado(a) como **desenvolvedor(a) web júnior** para auditar o site, identificar os problemas e entregar uma versão corrigida e melhorada, mantendo o conteúdo e a identidade visual básica, mas resolvendo:

1. **Erros de sintaxe** (código que não segue as regras de HTML/CSS);
2. **Erros estruturais** (uso incorreto de tags, hierarquia e organização do documento);
3. **Problemas de acessibilidade e experiência do usuário (UX)**.

---

## 2. Objetivos de aprendizagem

Ao final da atividade, o aluno deve ser capaz de:

- Ler e interpretar código HTML/CSS escrito por terceiros.
- Identificar e corrigir erros de sintaxe usando um validador (W3C Validator).
- Aplicar HTML semântico (`header`, `nav`, `main`, `section`, `footer` etc.) no lugar de `div`s genéricas.
- Corrigir hierarquia de títulos (`h1`–`h6`) e aninhamento inválido de elementos.
- Aplicar boas práticas de acessibilidade: `alt` em imagens, `label` em formulários, contraste de cores, foco visível, uso de `lang`.
- Tornar o layout responsivo com CSS (media queries, unidades relativas, `max-width`).

---

## 3. Habilidades trabalhadas (referência BNCC/Itinerário Formativo — Computação)

- Compreensão de estruturas de marcação e folhas de estilo.
- Depuração (*debugging*) de código.
- Design centrado no usuário e acessibilidade digital.
- Raciocínio lógico aplicado à organização de interfaces.

---

## 4. Materiais necessários

- Editor de código (VS Code ou similar).
- Navegador com DevTools.
- Acesso ao [W3C Markup Validator](https://validator.w3.org/) e [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/).
- Arquivos fornecidos: `./index.html` e `./style.css`.

---

## 5. Desenvolvimento da atividade

### Etapa 1 — Diagnóstico (auditoria)
Abra os arquivos fornecidos e preencha uma **tabela de auditoria** com pelo menos 10 problemas encontrados, classificando cada um em uma das três categorias:

| # | Problema encontrado | Categoria (Sintaxe / Estrutural / Acessibilidade-UX) | Linha aproximada | Como corrigir |
|---|---|---|---|---|
| 1 | | | | |

Dica: rode o HTML no [validador W3C](https://validator.w3.org/#validate_by_input) para listar os erros de sintaxe automaticamente.

### Etapa 2 — Correção
Reescreva o `index.html` e o `style.css` corrigindo os problemas listados na Etapa 1. Regras:

- Não pode remover conteúdo (textos, cursos, formulário) — apenas corrigir a estrutura.
- O HTML final deve ser validado sem erros no W3C Validator.
- O site deve usar pelo menos 5 tags semânticas do HTML5.
- Todo elemento interativo (links, botões, campos de formulário) deve ser acessível via teclado (Tab).
- O contraste de texto/fundo deve atingir no mínimo o nível **AA** do WCAG (relação de 4.5:1 para texto normal).

### Etapa 3 — Responsividade
Adicione pelo menos uma *media query* para que o site se adapte a telas de celular (largura até 480px), reorganizando o menu e ajustando larguras fixas para fluidas (`%`, `max-width`, `rem`).

### Etapa 4 — Justificativa técnica
Escreva um parágrafo curto (5 a 10 linhas) explicando as 3 mudanças que você considera mais importantes para a experiência do usuário e por quê.

---

## 6. Critérios de avaliação (rubrica)

| Critério | Insuficiente | Adequado | Excelente |
|---|---|---|---|
| Sintaxe válida | Site não valida no W3C, com múltiplos erros | Poucos erros restantes | 0 erros no validador |
| Estrutura semântica | Uso quase exclusivo de `div` | Uso parcial de tags semânticas | HTML5 semântico consistente, hierarquia de títulos correta |
| Acessibilidade | Sem `alt`, `label` ou contraste adequado | Corrige parte dos itens | Atende `alt`, `label`, contraste AA, navegação por teclado |
| Responsividade | Layout fixo, quebra em telas pequenas | Funciona parcialmente | Totalmente adaptável, com media query funcional |
| Justificativa técnica | Ausente ou genérica | Explica as mudanças superficialmente | Explica com domínio técnico e foco no usuário |

---

## 7. Desafio extra (opcional)
Adicionar um "pular para o conteúdo" (*skip link*) no topo da página e testar a navegação completa do site usando apenas o teclado (Tab, Shift+Tab, Enter).

---

## 8. Entregáveis
- `index.html` e `style.css` corrigidos.
- Tabela de auditoria preenchida (Etapa 1).
- Parágrafo de justificativa técnica (Etapa 4).
