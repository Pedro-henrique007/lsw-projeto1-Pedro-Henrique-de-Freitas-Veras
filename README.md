# Minha Loja - Game Station

Aluno(a): PEDRO HENRIQUE DE FREITAS VERAS - 202612010022

Como executar: node loja.js

Funcionalidades:

- `listarProdutos(lista)`: exibe cada produto em uma linha numerada a partir de 1, com nome, categoria, preço, quantidade em estoque e vendidos.
- `cadastrarProduto(lista, nome, categoria, preco, quantidade)`: cria um produto novo (com vendidos igual a 0 e nome formatado), adiciona ao final da lista e retorna a nova quantidade de produtos.
- `calcularValorEstoque(lista)`: retorna o valor total do estoque, somando preço × quantidade de todos os produtos.
- `buscarProduto(lista, termo)`: procura o primeiro produto cujo nome contém o termo, sem diferenciar maiúsculas de minúsculas. Retorna o produto ou `null`.
- `produtosEmFalta(lista, minimo)`: retorna um novo array com os produtos cuja quantidade é menor que o mínimo informado.
- `aplicarDesconto(lista, categoria, percentual)`: aplica o desconto no preço dos produtos da categoria e retorna quantos foram alterados.
- `registrarVenda(lista, nome, quantidade)`: registra a venda (diminui o estoque e aumenta os vendidos) e retorna `true`; retorna `false` se o produto não existir ou o estoque for insuficiente.
- `formatarNome(texto)`: remove os espaços das pontas, deixa a primeira letra maiúscula e o resto em minúsculas.
- `converterParaJSON(lista)`: converte o array de produtos em texto JSON.
- `lerJSON(texto)`: converte o texto JSON de volta em array.
- `gerarRelatorio(nome, lista)`: exibe o relatório da loja com o nome em maiúsculas, a quantidade de produtos, o valor total do estoque e a lista dos produtos com menos de 5 unidades.