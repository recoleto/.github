# 📖 Recoleto
Bem vindo a organização Recoleto! Desenvolvida para o Projeto Integrador II do Intituto Federal do Paraná - Campus Foz do Iguaçu. Aqui nesta organização você pode navegador pelos repositórios e commits feitos durante o desenvolvimento do projeto e ver sua evolução! Temos nas abas de repositórios, a camada de Lógica da API (repositório Recoleto-back-end) e a camada de Aplicação Web (repositório Recoleto-front-end). Neste documento, você terá um passo a passo de como acessar ele de maneira online e também localmente. Conheça nossa equipe!

<div align="center">
 <h2>🤝 Contribuidores</h2>
 <div display="inline-flex">
    <div align="center">
      <a href="https://github.com/gabrielamarqs" title="gabriela marques">
        <img src="https://avatars.githubusercontent.com/u/106118943?v=4" width="150px;" alt="Foto da Gabriela Marques no GitHub"/><br>
        <sub>
          <b>Gabriela Marques</b>
        </sub>
      </a>
     <p>Responsável pelo Back-end</p>
     <img src="https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/gabrielamarqs" />
     <img src="https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/gabriela-marques-dos-santos-899092161/" />
     <img src="https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white" />
    </div>
    <div align="center">
      <a href="https://github.com/mayspiek" title="mayara spieker">
        <img src="https://avatars.githubusercontent.com/u/79992764?v=4" width="150px;" alt="Foto da Mayara Spieker no Github"/><br>
        <sub>
          <b>Mayara Spieker</b>
        </sub>
      </a>
     <p>Responsável pelo Front-end</p>
     <img src="https://img.shields.io/badge/-Github-000?style=flat-square&logo=Github&logoColor=white&link=https://github.com/mayspiek" />
     <img src="https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/mayara-spieker/" />
     <img src="https://img.shields.io/badge/Gmail-red?style=flat-square&logo=gmail&logoColor=white" />
    </div>
</div>
</div>

<div align="center">
<h2>⚗️ Tecnologias</h2>
 <table>
  <td align="center">
   <p>Java</p>
   <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/java/java-original.svg" />    
  </td>
  <td align="center">
    <p>Spring Boot</p>
    <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg" /> 
  </td>
  <td align="center">
   <p>React Native</p>
   <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" /> 
  </td>
  <td align="center">
   <p>TypeScript</p>
    <img height="50em" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" />
  </td>
  <td align="center">
   <p>MySQL</p>
   <img height="50em" src="https://github.com/devicons/devicon/blob/v2.16.0/icons/mysql/mysql-original.svg" />
  </td>
 </table>
</div>

<!--  
### ✏️ Resumo
 <p align="justify">
   Entusiastas de leitura buscam formas de organizar o andamento de suas leituras de forma a manterem contato e engajamento com outras pessoas de interesses semelhantes. Embora existam diversos sistemas com uma ampla gama de funcionalidades, há uma carência de plataformas que oferecem uma visão centralizada e integrada das atividades de leitura. Este artigo apresenta o desenvolvimento do Shelfie, um Sistema de Gerenciamento e Monitoramento de Leituras, desenvolvido da necessidade dos usuários de poderem acompanhar e monitorar suas leituras diárias, a partir das progressões, do estado das leituras e das avaliações. Através de uma arquitetura de três camadas, desenvolvemos uma aplicação web separando a interface, lógica de negócios e dados. Isso facilita a manutenção para futuras melhorias. O Shelfie atingiu seus principais objetivos, que é oferecer uma interface para o usuário poder monitorar e gerenciar suas leituras a partir das funcionalidades implementadas. O projeto proporcionou importantes aprendizados sobre desenvolvimento de software e design centrado no usuário em aplicações Web.  
 </p>

 ## 🔗 Hospedagem
 A aplicação Web do Shelfie está hospedado em um Bucket AWS e está disponível para toda Web utilizar no seguinte link:
<a target="_blank" href="http://shelfiie-bucket.s3-website.us-east-2.amazonaws.com/">Shelfie</a>. Mas você também pode rodar localmente na sua máquina caso preferir. O tópico seguinte tratará sobre como instalar as dependências e como rodar a aplicação diretamente da sua máquina.

   -->
 ## 🛠️ Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

- Você instalou a versão mais recente do node e do npm para o front-end e para o back-end o java 17, o tomcat 10 e a última versão do MySQL.
- Você tenha git e vite instalado na sua máquina. 

### 💻 Instalando Shelfie-FrontEnd

Para instalar o Recoleto-FrontEnd, siga estas etapas:

Linux, macOS e Windows:

```
# clone o repositório
git clone https://github.com/recoleto/recoleto-front.git
# mova para o diretório da aplicação
cd /recoleto-front
# instale as dependências
npm install
```

### 🚀 Rodando o Shelfie-frontEnd
Para rodar a aplicação do Shelfie localmente é simples, basta você rodar o comando:
```
vite
```

### 💻 Instalando Shelfie-BackEnd

Para instalar o Recoleto-BackEnd, siga estas etapas:

Linux, macOS e Windows:

```
# acesse o MySQL como o usuário root
sudo mysql -u root -p
# crie o usuário do banco de dados
CREATE USER recoleto WITH PASSWORD 'Recoleto!2';
# crie o banco de dados
CREATE DATABASE tb_recoleto;
# conceda todas as permissões ao usuário recoleto para modificar o banco de dados criado
GRANT PRIVILEGE ON tb_recoleto.table TO 'recoleto'@'host';
GRANT CREATE, ALTER, DROP, INSERT, UPDATE, INDEX, DELETE, SELECT, REFERENCES, RELOAD on *.* TO 'recoleto'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;


# clone o repositório
git clone https://github.com/recoleto/recoleto-back.git
# mova para o diretório da aplicação
cd /recoleto-back
# Compile o projeto sem rodar os testes
mvn package -Dmaven.test.skip=true
```

### 🚀 Rodando o Recoleto-backEnd
Para rodar a API do Recoleto localmente é simples, basta você rodar o comando:
```
java -jar target/recoleto-0.0.1-SNAPSHOT.jar
```

E pronto! Sua aplicação deve rodar normalmente.

### 

