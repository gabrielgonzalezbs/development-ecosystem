
# Ecossistema de desenvolvimento

Este projeto serve como base para iniciar o desenvolvimento de  aplicações que utilizam o PHP e/ou Node. 


## Instalação

Faça o clone ou fork do projeto em sua máquina e ao concluir o load dos arquivos será necessário copiar e renomear o arquivo  `.env.example` para `.env`. Troque os dados das variaveis de ambiente para os números que desejar.

Após ter copiado renomeado o `.env` na raiz do seu projeto, basta executar o comando `docker compose build` para instalar os containers na sua máquina local. 

```bash
  docker compose build 
```

Se tudo correr bem, você podera exectuar o comando `docker compose up` e acessar os containers em sua máquina e instalar os projetos que deseja trabalhar.

```bash
  docker compose up 
```

Para acessar um container você pode utilizar o seguinte comando: 

```bash
docker compose exec php bash
```

Os seus projetos poderão ser criados e executados na pasta `applications/php` ou `applications/node`, dependendo é claro da linguagem que irá ser utilizada.
## Autor

- [@gabrielgonzalezbs](https://github.com/gabrielgonzalezbs)

