# Casos de Teste — Mercado Livre

## CT-001
**Título:** Validar login com sucesso utilizando credenciais válidas (e-mail e senha como forma de autenticação)
**Pré-condição:** O usuário deve possuir um cadastro ativo no sistema e estar na tela inicial de login
**Passos:**
1. Inserir o e-mail cadastrado no campo "E-mail"
2. Escolher a opção "Senha" como forma de autenticação
3. Inserir a senha correta no campo "Senha"
4. Clicar no botão "Confirmar"
**Dados de entrada:** Usuário: fulanodetal@xxx.com / Senha: SenhaSegura@123
**Resultado esperado:** O sistema deve autenticar o usuário, redirecioná-lo para o Dashboard e exibir a mensagem de boas-vindas: "Bem-vindo, Fulano"
**Resultado real:** O sistema autenticou o usuário e redirecionou para o dashboard / página inicial
**Status:** Passou

---

## CT-002
**Título:** Tentativa de validar login com senha incorreta
**Pré-condição:** O usuário deve possuir um cadastro ativo no sistema e estar na tela inicial de login
**Passos:**
1. Inserir o e-mail cadastrado no campo "E-mail"
2. Escolher a opção "Senha" como forma de autenticação
3. Inserir a senha incorreta no campo "Senha"
4. Clicar no botão "Confirmar"
**Dados de entrada:** Usuário: fulanodetal@xxx.com / Senha: SenhaIncorreta
**Resultado esperado:** O sistema deve exibir mensagem "Revise a sua senha"
**Resultado real:** O sistema exibiu a mensagem "Revise a sua senha"
**Status:** Passou

---

## CT-003
**Título:** Tentativa de validar login com campo de e-mail vazio
**Pré-condição:** O usuário deve estar na tela inicial de login
**Passos:**
1. Deixar o campo "E-mail" em branco
2. Clicar no botão "Continuar"
**Dados de entrada:** E-mail: vazio
**Resultado esperado:** O sistema deve impedir o login e exibir a mensagem de validação: "Preencha esse dado"
**Resultado real:** O sistema impediu o avanço e exibiu a mensagem: "Preencha esse dado"
**Status:** Passou

---

## CT-004
**Título:** Busca de itens com termos válidos
**Pré-condição:** O usuário deve estar devidamente autenticado no sistema e estar na tela inicial
**Passos:**
1. Inserir no campo de pesquisa (localizado na parte superior da tela) palavras para busca no sistema
2. Clicar na lupa (localizada no canto direito da caixa de pesquisa)
**Dados de entrada:** Campo de pesquisa: palavras que representam a busca desejada
**Resultado esperado:** O sistema deve filtrar e exibir todos os itens referentes à pesquisa realizada
**Resultado real:** O sistema filtrou a lista e exibiu 15 resultados correspondentes ao termo pesquisado, conforme o esperado
**Status:** Passou

---

## CT-005
**Título:** Tentativa de pesquisa no campo de "Busca" vazio
**Pré-condição:** O usuário deve estar devidamente autenticado no sistema e estar na tela inicial
**Passos:**
1. Deixar o campo "Busca" em branco
2. Clicar na lupa no canto direito da caixa de "Busca"
**Dados de entrada:** Campo de busca: vazio
**Resultado esperado:** O sistema deve exibir sugestões de itens recentemente pesquisados
**Resultado real:** O sistema exibiu uma lista suspensa com os últimos 5 itens pesquisados pelo usuário
**Status:** Passou

---

## CT-006
**Título:** Adicionar produto ao carrinho
**Pré-condição:** O usuário deve estar devidamente autenticado no sistema e estar na tela inicial
**Passos:**
1. Inserir no campo de pesquisa palavras para busca no sistema
2. Clicar na lupa no canto direito da caixa de pesquisa
3. Clicar no nome ou na imagem do produto nos resultados da busca para abrir a página de detalhes
4. Clicar no botão "Adicionar ao carrinho"
**Dados de entrada:** Campo de busca: item desejado a ser adicionado ao carrinho
**Resultado esperado:** O sistema deve confirmar a adição do item ao carrinho, exibindo a mensagem "Adicionado ao carrinho"
**Resultado real:** O sistema exibiu um pop-up com a mensagem "Adicionado ao carrinho" e o ícone do carrinho no topo da tela foi atualizado para "1"
**Status:** Passou

---

## CT-007
**Título:** Remover produto do carrinho
**Pré-condição:** O usuário deve estar autenticado e possuir itens previamente adicionados ao carrinho de compras
**Passos:**
1. Clicar no ícone de "Carrinho" no canto superior direito da tela inicial do sistema
2. Clicar no ícone de "Lixeira" localizado no final da descrição do produto que deseja excluir
**Dados de entrada:** Usuário: fulanodetal@xxx.com / Senha: SenhaSegura@123
**Resultado esperado:** O sistema deve confirmar a exclusão do item do carrinho, exibindo a mensagem "Pronto! Você excluiu o produto"
**Resultado real:** O sistema removeu o item da lista e exibiu a mensagem: "Pronto! Você excluiu o produto", conforme o esperado
**Status:** Passou
