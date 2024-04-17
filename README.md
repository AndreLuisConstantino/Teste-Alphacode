# Teste-Alphacode

## Instalação

1. Utilize o PHP versão: PHP 7.4.8.
2. Utilize Mysql versão: 5.7
3. Clone ou Fork o seguinte repositório: https://github.com/AndreLuisConstantino/Teste-Alphacode

## Configuração do banco de dados

Execute o seguinte script no seu workbench:

```sql
create database db_alphacode_contacts;
use db_alphacode_contacts;

create table tbl_contato(
	id int not null auto_increment primary key,
    nome varchar(150) not null,
    data_nascimento date not null,
    email varchar(255) not null,
    profissao varchar(150) not null,
    telefone varchar(15) not null,
    celular varchar(15) not null,
    tem_whatsapp boolean not null,
    notificacao_sms boolean not null,
    notificacao_email boolean not null,
    
    UNIQUE INDEX(id)
);
```

## Para inicializar o Projeto
1. Acese o arquivo ContatoDAO.php na pasta DAO e mude os dados sobre a conexão MySql para que coincidem com suas configurações.

2. Na pasta raiz do projeto execute o seguinte comando para iniciar o serviço: php -S localhost:8080

3. Acesse o 'localhost:8080' pela url do seu navegador e abra o site.

4. Agora a aplicação está pronta para uso,


