# Projeto de Prática – BANCO DE DADOS Elaboração de um modelo Entidade – Relacionamento

> [!Important]
> Entrega até dia 03/06.
>
> Fazer o ERD.
> 
> Salvar o script da tabela e das consultas e exportar. Um aluno do grupo envia pelo correio com o titulo: ENTREGA DO PROJETO DE PRÁTICA.



## 1 - Situação Problema: Sistema de Gerenciamento de Biblioteca:

Uma biblioteca deseja informatizar o seu sistema de gerenciamento de livros, usuários e empréstimos.
Atualmente, todas as operações são realizadas manualmente, e a biblioteca enfrenta desafios para
controlar o acervo, os empréstimos, as devoluções e as informações dos usuários. Para solucionar
esses problemas, a biblioteca decidiu implementar um sistema de banco de dados.

## Requisitos Funcionais:

### Livros:

- [ ] Cada livro possui um rotulo, um número de identificação único (ISBN), autor(es), editora e ano
de publicação.
- [ ] Deve ser possível cadastrar novos livros, atualizar informações e excluir registros.

### Usuários:

- [ ] Cada usuário possui um número de identificação único, nome, endereço, e-mail e telefone.
- [ ] O sistema deve permitir o cadastro de novos usuários, atualização de informações e exclusão
de registros.

 ### Empréstmos:
 
- [ ] Um empréstimo é associado a um usuário e a um livro específico.
- [ ] Cada empréstimo possui uma data de retirada e uma data de devolução prevista.
- [ ] Os empréstimos podem ser renovados, mas com um limite de renovações.
- [ ] O sistema deve gerenciar a disponibilidade dos livros para empréstmo.

### Devoluções:

- [ ] Quando um livro é devolvido, o sistema deve registrar a data da devolução.
- [ ] Deve ser possível verificar se um livro está atrasado e calcular eventuais multas.

### Restrições:

- [ ]  Um livro pode estar emprestado para apenas um usuário por vez.
- [ ]  Um usuário pode ter no máximo três livros emprestados simultaneamente.
- [ ]  Um usuário não pode ter mais de duas renovações para um mesmo livro.

## Tarefa:

Implementar um sistema de reserva, permitindo que usuários reservem livros que estão atualmente
emprestados. Caso um livro reservado seja devolvido, o sistema notifica o próximo usuário na fila de
espera.
Elabore um modelo de banco de dados usando o modelo Entidade-Relacionamento para atender a
esses requisitos. Identifique as entidades, atributos, relacionamentos e chaves primárias.

## Parte 2

## COMPLEXIDADE ADICIONAL PARA O SISTEMA DE BIBLIOTECA:

Adicione a capacidade de gerenciar diferentes filiais da biblioteca, onde cada filial possui seu próprio
conjunto de livros, usuários e registros de empréstimos. Cada livro pode estar disponível em uma ou
mais filiais, e os usuários podem ter cadastros em várias filiais. O sistema deve garantir que os
empréstimos e devoluções sejam registrados corretamente, considerando a localização do livro e do
usuário.

### Algebra Relacional:

Considere a necessidade de realizar consultas complexas para obter informações, como:

- [ ]  Encontrar todos os livros disponíveis em uma determinada filial.
- [ ]  Obter uma lista de usuários que têm livros emprestados em mais de uma filial.
- [ ]  Calcular o número total de livros disponíveis em todas as filiais.
