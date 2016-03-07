####API Produto.XYZ

API colaborativa de pesquisa de produtos por códigos de barras.

O objetivo principal do Produto XYZ é fornecer uma ampla base de dados de produtos e seus respectivos código de barras EAN. Hoje não existe nenhum centralizador deste tipo de dados, cada aplicativo tem sua base particular assim dificultando para desenvolvedores criar novos serviço que necessitem dos dados básicos de produtos.

######Versão

- v1 - Versão inicial [beta]
 - Pesquisa por código de barras.
 

####Documentação



######Consulta de um produto


API URI `https://api.produto.xyz/`

```
GET curl -k https://api.produto.xyz/7897312400184

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

[em desenvolvimento]
