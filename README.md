# Sistema de Cadastro/Login/Logout de usuários utilizando Sessões
Sistema simples de cadastro e login de usuários utilizando sessão implementado na linguagem Java com JSP, Servlet e banco de dados Oracle com JDBC 

## Preview

<table align="right">
  <tr>
    <td>
      <a href="readme-en.md">🇺🇸 English</a>
    </td>
  </tr>
  <tr>
    <td>
      <a href="README.md">🇧🇷 Português</a>
    </td>
  </tr>
</table>


<br>
<p align="center">
  <a href="#-apresentação-em-vídeo-do-projeto">Vídeo</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-tecnologias-utilizadas">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-sobre">Sobre</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-alguns-destaques">Destaques</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-clonando-o-projeto">Clone</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-contato-dos-contribuintes">Contato</a>
</p>
<br>





## 📹 Apresentação em Vídeo do Projeto
<div align="center">
  <video src="https://github.com/telsergio/CALCULADORA-SERGIO1/blob/main/VIDEO%20CALCULADORA%20SERGIO.mp4](https://github.com/telsergio/CALCULADORA-SERGIO1/assets/132212879/3feeb56d-e257-458c-94d2-bb3dbeb22e70">
</div>


## 🚀 Tecnologias Utilizadas

-   [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
-   [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
-   [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

## 📝 Sobre

> Assistir o vídeo acima e/ou acessar o projeto online ajudará na compreensão da explicação!

Para me aperfeiçoar mais na base do desenvolvimento Front-End, fiz esse projeto que se consiste numa Calculadora Web, desenvolvida utilizando o método `eval()` do Javascript como base.<br>
Lapidei principalmente meus conhecimentos em Javascript e CSS.

### 📌 Alguns Destaques

- Utilizei CSS Grid Layout para posicionar as partes da calculadora;
- Utilizei CSS Transition para fazer as animações;
- Utilizei variáveis CSS para padronizar a paleta de cores;
- Criei dois temas de cores com a possibilidade de alternância entre eles via Javascript;
- Fiz o mapeamento de todas as teclas equivalentes e a animação de feedback ao teclar via Javascript;


## 📹 Apresentação em Vídeo do Projeto
<div align="center">
  <video src="/github.com/telsergio/-Projeto-do-Login-Logout-by-Cookie-em-Servle/blob/main/Projeto%20do%20Login%20Logout%20by%20Cookie%20em%20Servlet2.mp4">
</div>



#### Cadastro
[![cadastro](https://github.com/telsergio/-Projeto-do-Login-Logout-by-Cookie-em-Servle/blob/main/cadastro.jpg)

#### Login
![login](https://github.com/telsergio/login-logout-jsp/raw/master/print/tela-login.png)


#### Mensagens de validação
[![validacao-login](https://github.com/XxJoaoQueirozxX/login-logout-jsp/raw/master/print/tela-login-validacao.png)](https://github.com/telsergio/-Projeto-do-Login-Logout-by-Cookie-em-Servle/blob/main/tela-login-validacao.png)

#### Página HOME (Renderezição dos dados do usuário)
![home](https://github.com/telsergio/login-logout-jsp/raw/master/print/home.png)



## Banco de Dados
**OBS**: Para efetuar a conexão com o banco de dados é necessário preencher os dados de conexão na classe ConnectionFactory localizada em **src/br/com/fiap/connection/ConnectionFactory.java**
você deve alterar os seguintes campos:
- dbURL: endereço do seu banco de dados(_exemplo: jdbc:oracle:thin:@localhost:1521:orcl_)
- user: Seu usuario no banco de dados
- pwd: A senha do seu usuário no banco 

Esse dados devem ser alterados no método abaixo:
![conexao](https://github.com/telsergio/login-logout-jsp/raw/master/print/conexao.png)

### Script SQL para criação das tabela e sequence (Oracle DB)
script sql para a criação da tabela de usuário no banco de dados e a sequence relativa a seu id

    CREATE TABLE TBL_LOGIN(
        id_user number(10) not null,
        nome varchar(100) not null,
        nm_user varchar2(300) not null,
        pass_user varchar2(300) not null,
        url_avatar varchar2(1000) not null,
        CONSTRAINT login_pk PRIMARY KEY (id_user)
    );
    create sequence seq_login
    minvalue 1
    maxvalue 99999999999
    start with 1
    increment by 1
    nocache
    cycle;
