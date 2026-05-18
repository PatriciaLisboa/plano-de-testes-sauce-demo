# Guia de prática semanal — QA Manual na Sauce Demo

## Antes de começar

Acesse https://www.saucedemo.com e explore a aplicação livremente.
Os usuários de teste disponíveis são:

| Usuário | Senha | Comportamento |
|---|---|---|
| standard_user | secret_sauce | Funciona normalmente |
| locked_out_user | secret_sauce | Está bloqueado |
| problem_user | secret_sauce | Tem bugs visuais |
| performance_glitch_user | secret_sauce | Carrega com lentidão |

---

## Dia 1 — Explorar a aplicação

- Acesse a Sauce Demo e navegue sem objetivo definido
- Tente fazer login com cada usuário da tabela acima
- Anote tudo que chamar atenção — comportamentos estranhos, mensagens
  de erro, elementos que parecem errados
- Não precisa documentar nada formalmente ainda, só observar

---

## Dia 2 — Escrever o plano de testes

O plano de testes é o documento que define o que será testado e como.
Crie o arquivo `plano-de-testes/plano-geral.md` respondendo:

- Qual é o objetivo dos testes?
- Quais funcionalidades serão testadas? (login, carrinho, checkout)
- Quais funcionalidades estão fora do escopo?
- Quais tipos de teste serão feitos? (funcional, regressão)
- Quais navegadores e sistemas serão usados?
- Quais são os critérios para considerar um teste bem-sucedido?

---

## Dia 3 — Escrever casos de teste de login

Use o template em `templates/template-caso-de-teste.md` e crie
os seguintes casos dentro da pasta `casos-de-teste/`:

- `CT001-login-usuario-valido.md` — login com standard_user
- `CT002-login-usuario-bloqueado.md` — login com locked_out_user
- `CT003-login-senha-incorreta.md` — login com senha errada
- `CT004-login-campos-vazios.md` — clicar em login sem preencher nada

Para cada caso preencha todos os campos do template e execute o teste
na aplicação para anotar o resultado obtido.

---

## Dia 4 — Escrever casos de teste de carrinho

Crie os seguintes casos dentro da pasta `casos-de-teste/`:

- `CT005-adicionar-produto-carrinho.md`
- `CT006-remover-produto-carrinho.md`
- `CT007-carrinho-vazio.md`

Acesse a Sauce Demo com standard_user e execute cada caso enquanto
documenta.

---

## Dia 5 — Documentar bugs encontrados

Durante os dias anteriores você deve ter encontrado comportamentos
inesperados, especialmente com problem_user e locked_out_user.
Use o template em `templates/template-bug-report.md` e crie
um bug report para cada problema encontrado dentro da pasta
`bug-reports/`.

Tire prints de cada bug como evidência e salve na pasta `evidencias/`.

