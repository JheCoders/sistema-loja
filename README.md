# Sistema ENSINA LOJA

## Descrição

O Sistema ENSINA LOJA é uma aplicação desenvolvida em Python para gerenciamento de informações de uma loja utilizando um banco de dados MySQL. O sistema permite realizar operações de consulta, inserção, atualização e exclusão (CRUD) de clientes e produtos, além de visualizar dados de outras tabelas relacionadas aos pedidos e ao inventário.

## Funcionalidades

### Gerenciamento de Clientes
- Listar clientes cadastrados.
- Inserir novos clientes.
- Editar informações de clientes existentes.
- Excluir clientes.

### Gerenciamento de Produtos
- Listar produtos cadastrados.
- Inserir novos produtos.
- Editar informações de produtos existentes.
- Excluir produtos.

### Consultas
- Visualizar dados da tabela Inventário.
- Visualizar dados da tabela ItensPedido.
- Visualizar dados da tabela Pedidos.

### Banco de Dados
- Conexão automática com o servidor MySQL.
- Fechamento seguro da conexão ao finalizar a aplicação.
- Tratamento de erros durante as operações no banco de dados.

## Tecnologias Utilizadas

- Python 3
- MySQL
- Biblioteca `mysql-connector-python`

## Instalação

Antes de executar o programa, instale a biblioteca necessária:

```bash
pip install mysql-connector-python
```

## Configuração do Banco de Dados

O sistema utiliza os seguintes parâmetros de conexão:

| Parâmetro | Valor |
|------------|--------|
| Host | db4free.net |
| Banco de Dados | aprendizadosql |
| Usuário | profdurval |

> A senha do banco está definida diretamente no código.

## Estrutura do Projeto

| Função | Descrição |
|----------|-----------|
| `connect_to_database()` | Realiza a conexão com o MySQL. |
| `execute_select_query()` | Executa consultas SELECT em qualquer tabela. |
| `inserir_cliente()` | Cadastra um novo cliente. |
| `editar_cliente()` | Atualiza os dados de um cliente. |
| `excluir_cliente()` | Remove um cliente do banco. |
| `inserir_produto()` | Cadastra um novo produto. |
| `editar_produto()` | Atualiza os dados de um produto. |
| `excluir_produto()` | Remove um produto do banco. |
| `menu_clientes()` | Exibe o menu de operações de clientes. |
| `menu_produtos()` | Exibe o menu de operações de produtos. |
| `main_menu()` | Controla o menu principal do sistema. |

## Menu Principal

Ao iniciar o programa, o usuário terá acesso às seguintes opções:

```text
*** SISTEMA ENSINA LOJA ***

1. Ações em Clientes
2. Ações em Produtos
3. Exibir dados da tabela Inventário
4. Exibir dados da tabela ItensPedido
5. Exibir dados da tabela Pedidos
6. Finalizar
```

## Como Executar

1. Salve o código em um arquivo chamado:

```bash
sistema_loja.py
```

2. Instale a dependência:

```bash
pip install mysql-connector-python
```

3. Execute o programa:

```bash
python sistema_loja.py
```

## Exemplo de Uso

### Inserindo um Cliente

```text
Digite o nome do cliente: João Silva
Digite o email do cliente: joao@email.com
Digite o endereço do cliente: Rua das Flores, 100

Cliente inserido com sucesso!
```

### Inserindo um Produto

```text
Digite o nome do produto: Notebook
Digite a descrição do produto: Notebook Dell Inspiron
Digite o preço do produto: 3500

Produto inserido com sucesso!
```

## Tratamento de Erros

O sistema possui tratamento de exceções para:

- Falhas na conexão com o banco de dados.
- Erros durante consultas.
- Problemas nas operações de inserção, atualização e exclusão.

## Autor

Desenvolvido por **James Kawen Guedes de Sousa**.

## Licença

Este projeto foi desenvolvido para fins educacionais e pode ser utilizado, modificado e distribuído livremente.
