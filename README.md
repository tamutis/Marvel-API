# Marvel-API

Este repositório contém testes automatizados da API da Marvel utilizando o Postman. Os testes são executados através do Newman e geram relatórios de testes detalhados.

## Pré-requisito

Node:
```
https://nodejs.org/en/download/
```

Newman:
```
npm install -g newman-reporter-html-extra
```

Para executar os testes usando o Newman no terminal, você pode utilizar o seguinte comando:
```
newman run "Marvel API.postman_collection.json" -e "MarvelEnviorement.postman_environment.json" -r htmlextra --reporter-html-export test-report.html

```