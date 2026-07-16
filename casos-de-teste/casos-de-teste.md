# Casos de Teste

Este documento apresenta os casos de teste executados durante a validação das principais funcionalidades do Sauce Demo. Todos os cenários descritos foram executados com sucesso no ambiente de testes.

| ID     | Cenário                     | Resultado Esperado                                                                              | Status   |
| ------ | --------------------------- | ----------------------------------------------------------------------------------------------- | -------- |
| CT-001 | Login válido                | O usuário deverá acessar o sistema e ser redirecionado para a página de produtos.               | Aprovado |
| CT-002 | Senha inválida              | O sistema deverá impedir o login e apresentar uma mensagem de erro ao usuário.                  | Aprovado |
| CT-003 | Usuário inválido            | O sistema deverá impedir o login e apresentar uma mensagem de erro ao usuário.                  | Aprovado |
| CT-004 | Usuário vazio               | O sistema deverá solicitar o preenchimento do campo de usuário.                                 | Aprovado |
| CT-005 | Senha vazia                 | O sistema deverá solicitar o preenchimento do campo de senha.                                   | Aprovado |
| CT-006 | Adicionar produto           | O produto selecionado deverá ser adicionado corretamente ao carrinho de compras.                | Aprovado |
| CT-007 | Remover produto             | O produto selecionado deverá ser removido corretamente da lista de produtos.                    | Aprovado |
| CT-008 | Visualizar produto          | As informações do produto deverão ser apresentadas corretamente ao usuário.                     | Aprovado |
| CT-009 | Ordenar produtos            | Os produtos deverão ser ordenados corretamente conforme o filtro selecionado.                   | Aprovado |
| CT-010 | Remover produto do carrinho | O produto deverá ser removido corretamente do carrinho de compras.                              | Aprovado |
| CT-011 | Continuar comprando         | O usuário deverá retornar à página de produtos para continuar a navegação.                      | Aprovado |
| CT-012 | Checkout válido             | O processo de compra deverá ser concluído com sucesso.                                          | Aprovado |
| CT-013 | Nome vazio                  | O sistema deverá impedir o avanço do checkout e solicitar o preenchimento do campo obrigatório. | Aprovado |
| CT-014 | Sobrenome vazio             | O sistema deverá impedir o avanço do checkout e solicitar o preenchimento do campo obrigatório. | Aprovado |
| CT-015 | CEP vazio                   | O sistema deverá impedir o avanço do checkout e solicitar o preenchimento do campo obrigatório. | Aprovado |
| CT-016 | Logout                      | O usuário deverá ser desconectado do sistema e retornar à tela inicial de login.                | Aprovado |
