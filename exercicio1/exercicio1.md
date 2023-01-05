# Exercício 1
Hoje nosso foco será **refatorar** nossos endpoints do Labecommerce e torná-los mais robustos e preparados para lidar com erros.

## Get All Users
- verificar se existem users
    - caso não existam, retornar uma mensagem de erro apropriada

## Get All Products
- verificar se existem products
    - caso não existam, retornar uma mensagem de erro apropriada

## Search Product by name
- tratar a entrada (query params), para que nosso endpoint não diferencie letras maiúsculas e minúsculas (por exemplo, nosso programa deve lidar com os termos "Camiseta" e "camiseta" da mesma forma)
- verificar se existem products com o termo da busca
    - se não existirem, retornar uma mensagem de erro apropriada

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