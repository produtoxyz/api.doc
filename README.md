![ProdutoXYZ](https://github.com/produtoxyz/api/blob/master/produto-xyz.png)


API colaborativa de pesquisa de produtos por códigos de barras GTIN.

O objetivo principal do Produto XYZ é fornecer uma ampla base de dados de produtos e seus respectivos código de barras EAN. Hoje não existe nenhum centralizador deste tipo de dados, cada aplicativo tem sua base particular assim dificultando para desenvolvedores criar novos serviço que necessitem dos dados básicos de produtos.

####Documentação

#### Get products
`$ curl -XGET https://api.produto.xyz/v1/gtin/{codebar}`


Busca por GTIN

```
$ curl --location --request GET 'https://produto.xyz/v1/gtin/7897312400184'
Response:
{
   Product: {
      gtin: "7897312400184",
      name: "DETERGENTE ECONOMICO NEUTRO 500ML",
      category: "",
      manufacturer: "",
      id: "9587e7802342424234"
   }
}
```

Busca por nome

```
curl --location --request GET 'http://produto.xyz/v1/gtin?q=sabao%20cra%20cra'
Response:
{
   "paging": {
       "total": 3,
       "offset": 0,
       "limit": 50,
   },
   {...},
   {...},
   {...}
}
```

-----------------
#####Changelogs

## v1 

###0.0.1 [alpha]


"Milagres acontecem, retomando esta idéia com novas idéias e tecnologias...." 
