# psi-pratica2-Hugley

1. Para que serve disponivel?
Serve como um indicador de estado do livro para controlar o fluxo de empréstimo e devolução no sistema. Sendo um valor booleano, ele permite filtrar facilmente quais livros estão prontos para serem emprestados aos leitores e impede que um mesmo livro seja emprestado duas vezes seguidas.

2. Por que usar session.commit()?
O session.commit() serve para persistir definitivamente as alterações no banco de dados. Até o momento em que você chama o commit(), todas as operações como criar registros, alterar atributos ou remover itens acontecem apenas na memória temporária da sessão SQLAlchemy. O commit() envia a transação SQL final ao banco, garantindo a gravação dos dados.

3. Em qual consulta você usa o relacionamento entre `Livro` e `Autor`?
Em livro.autor.nome: Para pegar o nome do autor direto do livro, em autor.livros: Para listar todos os livros de um autor específico, ao cadastrar: Para ligar cada livro ao seu autor através do autor_id.
