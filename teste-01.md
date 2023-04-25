# Teste 1 - Checkout

Imagine o seguinte cenário: Você é um desenvolvedor em uma empresa de e-commerce que entrega seus serviços através de um monolíto. Porém, o módulo de checkout da empresa está recebendo muitos acessos e o sistema não consegue dar conta da demanda. Por conta disso, chega uma tarefa no seu backlog com a descrição abaixo.

OBS: O checkout é a parte do sistema que computa os produtos adicionados a um carrinho de compras e retorna o preço.

## Requisitos encontrados no backlog

- É preciso que um novo sistema seja desenvolvido de forma ele possa ser consumido na forma de uma API REST pelos outros módulos da empresa.
- Esse novo sistema precisa aceitar como input - uma lista com o id dos produtos, o cpf do cliente e um cupon se existir.
- A aplicação deve garantir que o cpf do cliente seja válido.
- Ao realizar o checkout o sistema deveretornar o valor da compra que será efetuada.

É desejável que o sistema tenha seu funcionamento e qualidade garantidos por meio de testes (sejam eles quais forem).
