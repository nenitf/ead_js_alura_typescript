# ead_js_alura_typescript

> Projeto referente a [este](https://cursos.alura.com.br/course/typescript-evoluindo-javascript), [este](https://cursos.alura.com.br/course/typescript-avancando-linguagem) e [este](https://cursos.alura.com.br/course/typescript-tecnicas-boas-praticas) cursos.

1. Crie o ambiente
```sh
docker-compose up -d
```
> Caso queira, ao final da configuração, pare o Docker com ``docker-compose down``

2. Baixe as dependências
```sh
docker-compose exec app npm i
```

3. Acesse o projeto e baixe as dependências do servidor falso
```sh
docker-compose exec app bash
```
```sh
cd servidor-api
npm i
```

## Execução

1. Suba o ambiente
    - Caso recém tenha feito a **configuração inicial** e o ambiente continue rodando, tudo certo.
    - Do contrário, suba o ambiente novamente: ``docker-compose up -d``

2. Inicie o servidor do projeto
```sh
docker-compose exec app npm start
```

3. Com outro terminal, inicie o servidor falso
```sh
docker-compose exec app bash
```
```sh
cd servidor-api
npm start
```

4. Acesse ``localhost:3000``
