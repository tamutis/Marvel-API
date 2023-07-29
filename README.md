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

Report:
![Captura de Tela 2023-07-29 às 15 51 15](https://github.com/tamutis/marvel-api-collection/assets/20347604/7f443870-27dd-4914-b722-60377d4a1046)


## Integração Contínua com GitHub Actions

Este projeto está configurado com o GitHub Actions para automatizar a execução dos testes. Os testes são agendados para serem executados em horários específicos usando uma expressão cron.

### Agenda dos Testes

Os testes serão executados nos seguintes horários todos os dias:

- 9:00 AM
- 12:00 PM
- 3:00 PM
- 6:00 PM
- 9:00 PM

