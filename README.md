# Trabalho-Sistema-Mercado

1. Inclusão de Bibliotecas
   
#include <stdio.h>
#include <string.h>

Aqui, duas bibliotecas padrão são incluídas:
stdio.h: para entrada e saída padrão (funções como printf e scanf).
string.h: para manipulação de strings, embora não seja utilizada de forma explícita no código.

2. Definições e Estruturas

#define MAX_PRODUTOS 50
#define MAX_CARRINHO 50

Esses #define definem constantes que limitam o número máximo de produtos e itens no carrinho.

typedef struct {
    int codigo;
    char nome[30];
    float preco;
    int quantidadep;
} Produto;

typedef struct {
    Produto produto;
    int quantidade;
} Carrinho;

Duas estruturas são definidas:

Produto: contém informações sobre o produto (código, nome, preço e quantidade).
Carrinho: contém um Produto e a quantidade desse produto no carrinho.

3. Declaração de Variáveis Globais

Produto produtos[MAX_PRODUTOS];
Carrinho carrinho[MAX_CARRINHO];
int totalProdutos = 0;
int totalCarrinho = 0;

Aqui, arrays para armazenar produtos e itens do carrinho são declarados, juntamente com contadores para rastrear quantos produtos e itens estão registrados.

4. Declaração de Funções
   
Um conjunto de funções é declarado, cada uma responsável por uma operação específica:

menu(): exibe o menu principal.
cadastrarProduto(): permite o cadastro de novos produtos.
listarProdutos(): lista os produtos cadastrados.
comprarProduto(): adiciona produtos ao carrinho.
visualizarCarrinho(): exibe os itens no carrinho.
fecharPedido(): finaliza a compra e exibe o total.
temNoCarrinho(int codigo): verifica se um produto já está no carrinho.
pegarProdutoPorCodigo(int codigo): busca um produto pelo seu código.
infoproduto(): imprime informações dos produtos cadastrados.

5. Função Principal

int main() {
    menu();
    return 0;
}
A função main inicia o programa chamando a função menu().

6. Função do Menu

void menu() {
    // Código para exibir opções e capturar a escolha do usuário
}
O menu exibe opções ao usuário, permitindo que ele escolha o que deseja fazer (cadastrar produtos, listar, comprar, etc.). O loop continua até que o usuário escolha sair.

7. Cadastrar Produto

void cadastrarProduto() {
    // Código para cadastrar produtos
}
Permite que o usuário cadastre múltiplos produtos, verificando se o limite não foi atingido.

8. Listar Produtos

void listarProdutos() {
    // Código para listar produtos cadastrados
}
Exibe todos os produtos cadastrados, ou informa se não há produtos.

9. Comprar Produto

void comprarProduto() {
    // Código para adicionar produtos ao carrinho
}
Permite que o usuário adicione um produto ao carrinho, verificando se ele já existe no carrinho e atualizando a quantidade se necessário.

10. Visualizar Carrinho

void visualizarCarrinho() {
    // Código para mostrar os itens no carrinho
}
Exibe todos os produtos atualmente no carrinho de compras.

11. Fechar Pedido

void fecharPedido() {
    // Código para finalizar a compra
}
Calcula e exibe o total da compra, esvaziando o carrinho ao final.

12. Funções Auxiliares
infoptroduto: imprime as informações dos produtos cadastrados pelo usuário.
temNoCarrinho: verifica se um produto já está no carrinho.
pegarProdutoPorCodigo: retorna um ponteiro para um produto correspondente ao código fornecido.




Não compartilhe informações confidenciais. Os chats podem ser revisados e usados para treinar nossos modelos. Saiba mais


