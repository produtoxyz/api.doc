![ProdutoXYZ](https://github.com/produtoxyz/api/blob/master/produto-xyz.png)


API colaborativa de pesquisa de produtos por códigos de barras.

O objetivo principal do Produto XYZ é fornecer uma ampla base de dados de produtos e seus respectivos código de barras EAN. Hoje não existe nenhum centralizador deste tipo de dados, cada aplicativo tem sua base particular assim dificultando para desenvolvedores criar novos serviço que necessitem dos dados básicos de produtos.

####Documentação

#### Get products
`$ curl -XGET https://api.produto.xyz/{codebar}`

```
$ curl -XGET https://api.produto.xyz/7897312400184
Response:
{
   Product: {
      barcode: "7897312400184",
      name: "DETERGENTE ECONOMICO NEUTRO 500ML",
      category: "",
      manufacturer: "",
      id: "9587e780-e495-11e5-9d5b-5da257427e93"
   }
}
```



#### Add products
```
$ curl -XPOST https://api.produto.xyz/v1/products \
       -H 'Content-Type: application/json' \
       -d '{"": ""}'
```
#### Update products
```
$ curl -XPUT https://api.produto.xyz/v1/products/{id} \
        -H 'Content-Type: application/json' \
        -d '{"": "."}'
```

#### Delete products
`$ curl -XDELETE https://api.produto.xyz/v1/products/{id}`


-----------------
#####Changelogs

## v1 

###1.0.0 [beta]
  * teste.


[em desenvolvimento]

