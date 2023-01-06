# Exercício 1
Hoje nosso foco será **refatorar** nossos endpoints do Labecommerce e torná-los mais robustos e preparados para lidar com erros.

## Get All Users
- não precisa de validação, basta refatorar para o uso do try/catch

## Get All Products
- não precisa de validação, basta refatorar para o uso do try/catch

## Search Product by name
- query params deve possuir pelo menos um caractere

## Create User
- verificar se todos os dados do body foram informados e seus respectivos tipos
    - caso o body esteja incompleto e/ou incorreto, retorne uma mensagem de erro apropriada
- verificar se existe outro user com o mesmo email
    - caso exista, retornar mensagem de erro apropriada

## Create Product
- verificar se todos os dados do body foram informados e seus respectivos tipos
    - caso o body esteja incompleto e/ou incorreto, retorne uma mensagem de erro apropriada
- verificar se existe outro product com o mesmo nome
    - caso exista, retornar mensagem de erro apropriada

## Create Purchase
- verificar se todos os dados do body foram informados e seus respectivos tipos
    - caso o body esteja incompleto e/ou incorreto, retorne uma mensagem de erro apropriada
- verificar se realmente existe um user com o userId informado
    - caso não exista, retorne uma mensagem de erro apropriada
- verificar se realmente existe um product com o productId informado
    - caso não exista, retorne uma mensagem de erro apropriada
