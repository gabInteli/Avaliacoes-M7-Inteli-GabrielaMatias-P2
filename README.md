# Avaliação 2 - Gabriela Rodrigues Matias 

A seguir apresentarei um passo a passo de como foi executada a atividade para a avaliação 2, seguida dos comandos necessários para rodar essa aplicação; 

## Criação de Banco RDS
Para iniciar o projeto foi criado um banco de dados com RDS para poder fazer o armazenamento de todas as informações do sistema. Conforme demonstrado na sequência de imagens abaixo: 
![Create RDS](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/criar-rds.png)

### Teste de Conexão 
![Teste Conexao DB](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/teste-conexao-db.png)

## Criação de Instância 1 - EC2: Backend
Para poder executar nosso backend, criamos uma instância no EC2 para executar nosso backend. 
![Criar Instância do Backend](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/criando-instancia1.png)
![Criar Instância do Backend](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/instancia1-criada.png)

## Criação de Instância 2 - EC2: Frontend
Para poder executar nosso frontend, criamos uma instância no EC2 para executar nosso servidor de interface. 
![Criar Instância do Frontend](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/instancia2-criando.png)
![Criar Instância do Frontend](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/instancia2-criada.png)

## Execução - Backend 
Inicialmente foi feito um clone do repositório principal. Antes disso, foram alteradas as rotas do backend para apontarem para o banco de dados desenvolvido utilizando o RDS. 
Em seguida, foram instaladas todas as dependências necessárias para o backend seguindo o arquivo `requirements.txt`. 

Por fim, foi criado o banco de dados: 
![Criar DB](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/criar-db.png)

E em seguida, foi executado o servidor em FastAPI: 
![Rodar Servidor](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/running-server.png)

### Teste - Postman
Para validar o funcionamento do servidor, foi feito um teste utilizando o Postman: 

#### Post - Dados
![Teste com Postman](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/teste-envio-nota-postman.png)

#### Get - Dados 

![Teste com Postman](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/validacao-teste-nota.png)

## Execução - Frontend
Para executar o nosso front inicialmente foi criado um server com apache na Instância. 
Em seguida foi criado um arquivo: `front.html`

Por fim, foi acessado o servidor que continha esse front de dados, conforme a demonstração abaixo. 
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/update-front.png)

## Demonstração 
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/tela-front.png)
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/run-front.png)
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/frontend.png)
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/post.png)
![Front](https://github.com/gabInteli/Avaliacoes-M7-Inteli-GabrielaMatias-P2/blob/main/media/delete.png)

