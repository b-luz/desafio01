# Teste 1 - Checkout

Olá, dev! 

Se você chegou até aqui, significa que está avançado no processo seletivo técnico do Bluz. E por isso, nossos sinceros parabéns! 🥳

Essa é a última etapa do processo seletivo, o code challange 🥋. Todas as instruções de entrega e requisitos do desafia estão descritos abaixo, portanto, **leia com atenção**.

## Instruções para execução e entrega

- 🗓️ Prazo: 3 dias de quando foi passado o teste;
- 📄 Desenvolvimento: crie um repositório público no seu github e desenvolva o projeto nele (em qualquer linguagem ou framework);
- ✅ Entrega: mande o link do repositório do projeto para gabriel.lopes@baptistaluz.com.br com seu nome completo;

## Critérios de avaliação 

Nesse desafio serão avaliados: seu senso crítico e habilidade de resolução de probelemas, organização e qualidade de código.

🔴 Não tem problema se não você não conseguir finalizar à tempo, o importante é que seja enviado o projeto com a lógica da aplicação.

---

# Problema

Imagine o seguinte cenário: Você é um desenvolvedor em uma empresa de e-commerce que entrega seus serviços através de um monolíto. Porém, o módulo de checkout da empresa está recebendo muitos acessos e o sistema não consegue dar conta da demanda. Por conta disso, chega uma tarefa no seu backlog com a descrição abaixo.

OBS: O checkout é a parte do sistema que computa os produtos adicionados a um carrinho de compras e retorna o preço.

Tanto a lista de produto quanto a lista de cupons podem ser implementados em memória.

## Requisitos encontrados no backlog

- É preciso que um novo sistema seja desenvolvido de forma ele possa ser consumido na forma de uma API REST pelos outros módulos da empresa.
- Esse novo sistema precisa aceitar como input - uma lista com o id dos [produtos](#produtos), o cpf do cliente e um [cupom](#cupom) se existir.
- Ao realizar o checkout o sistema deve retornar o valor da compra que será efetuada aplicando o cupom e o valor do frete.
- Um cupom deve ser aplicado somente se existir e estiver dentro da data de validade. Caso contrário deve ser ignorado.
- O frete deve ser calculado usando a fórmula: Frete = peso * 0.1.
- O checkout não pode ser efetuado caso o cpf do cliente seja inválido.
- O checkout não pode ser efetuado caso haja um produto duplicado ou inexistente.
- É desejável que o sistema tenha seu funcionamento e qualidade garantidos por meio de testes (sejam eles quais forem).

## Lista de <a name="produtos">produtos</a>

| id | name | price | weight (kg)
| ---| --- | --- | --- |
| 1  | Livro Clean Code | 120.00 | 0.2
| 2  | Assinatura Amazon | 19.90 | 0
| 3  | Mouse gamer RGB | 50.00 | 0.1
| 4  | Monitor 34 polegadas | 500.00 | 5.0
| 5  | Cadeira de balanço | 78.90 | 10.0
| 6  | Skate | 180.50 | 3.0


## Lista de <a name="cupom">cupons</a>

| code | discount_percentage | expires_at |
| ---| --- | --- |
| ABC10 | 10 | 2080-10-05 00:00:00
| XYZ05 | 5 | 2080-10-05 00:00:00
| QWE20 | 20 | 2020-03-10 00:00:00

