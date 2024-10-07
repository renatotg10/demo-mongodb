# MongoDB Demo Script

Este repositório contém um exemplo de script em Node.js que utiliza o driver oficial do MongoDB para listar todos os bancos de dados de um cluster MongoDB.

## Descrição

O arquivo `demo.js` é um script simples que se conecta a um cluster MongoDB utilizando o **MongoDB Atlas** e lista os bancos de dados disponíveis no console. Ele usa o pacote `mongodb` para estabelecer a conexão e executar as operações no banco de dados.

## Requisitos

Para executar este script, você precisa ter:

- Node.js instalado (versão 14.x ou superior)
- Uma conta no [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) ou um cluster MongoDB local
- O pacote `mongodb` instalado no projeto

## Instalação

1. Clone este repositório para sua máquina local:
    ```bash
    git clone https://github.com/seu-usuario/mongodb-demo.git
    cd mongodb-demo
    ```

2. Instale as dependências:
    ```bash
    npm install mongodb
    ```

## Configuração

1. Abra o arquivo `demo.js` e substitua a string de conexão (`uri`) pelas suas credenciais MongoDB. Atualize os seguintes valores:
    ```javascript
    const uri = "mongodb+srv://<usuario>:<senha>@<usuario>.m2yvc.mongodb.net/?retryWrites=true&w=majority&appName=<usuario>";
    ```
   - Substitua `<usuario>` pelo seu nome de usuário do MongoDB.
   - Substitua `<senha>` pela sua senha do MongoDB.

2. Salve o arquivo.

## Execução

Para executar o script e listar os bancos de dados no console, utilize o comando abaixo no terminal:

```bash
node demo.js
```

Se a conexão for bem-sucedida, o script retornará algo como:

```
Databases:
- admin
- local
- myDatabase
```

## Recursos

- **MongoDB Atlas**: É uma solução de banco de dados em nuvem que facilita o gerenciamento e a escalabilidade de clusters MongoDB. Saiba mais [aqui](https://www.mongodb.com/cloud/atlas).
- **Node.js**: Ambiente de execução Javascript para desenvolvimento de aplicações em backend. Saiba mais [aqui](https://nodejs.org/en/).

## Problemas Comuns

- **Erro de Autenticação**: Se houver um erro de autenticação, verifique se as credenciais na URI de conexão estão corretas.
- **Erro de Conexão**: Verifique se a sua instância MongoDB está acessível, e se você está permitindo acessos de IPs externos em suas configurações do MongoDB Atlas.

## Licença

Este projeto está licenciado sob os termos da licença MIT.

## Referências:

https://www.mongodb.com/developer/languages/javascript/node-connect-mongodb/

https://youtu.be/fbYExfeFsI0?si=Daaj8OfM3RxMFhm9
