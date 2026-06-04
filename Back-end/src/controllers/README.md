Parte feita por: Pyetro

No arquivo authController eu desenvolvi o fluxo de autenticação simulada que valida credenciais de acesso (admin / 123456).
e implementei a geração automática de um token criptografado temporariamente contendo o ID e o timestamp real do login, blindando a sessão e retornando as iniciais do usuário logado para o Front-end.

Em movimentacaoController criei a listagem de todas as auditorias físicas, utilizando relacionamentos do Prisma para carregar o nome legível de cada insumo. Desenvolvi o cálculo inteligente para as movimentações. O sistema avalia dinamicamente a string recebida:
Se for identificado o tipo ENTRADA, o sistema faz o incremento automático do saldo no estoque.
Se for identificado o tipo SAÍDA, o sistema inverte o valor para negativo e decrementa automaticamente o saldo final, utilizando funções nativas do banco via Prisma.

E em produtoController implementei a persistência e listagem completa dos medicamentos catalogados no sistema (nomes, marcas, preços e unidades). Para evitar erros de dados órfãos ou quebras de integridade no banco, desenvolvi uma Transação Atômica. Quando um medicamento é deletado, o controlador limpa simultaneamente e obrigatoriamente todas as referências associadas a ele nas tabelas de Movimentacao, Reposicao e ItemPedido antes de remover o produto definitivo.