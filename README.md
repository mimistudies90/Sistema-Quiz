# Sistema-Quiz
# Modelo de Documentação para Aplicação PHP com MySQL


## 1 Introdução
    • **Nome do Projeto:** [Sistema_Quiz]
    • **Descrição:** [OO *Sistema_quiz** é um projeto desenvolvido para fãs de animes que desejam desafiar sua memória e expertise. O sistema oferece perguntas categorizadas por dificuldade, garantindo diversão tanto para iniciantes quanto para experts ]
    • **Tecnologias Utilizadas:** PHP, MySQL, HTML, CSS, JavaScript,Visula Studio Code
    • **Autor(es):** [aria Conceição, Yasmin Moreira, Ravisya Narciso, Julia Carmo.   ]
    • **Data de início:** [17/03/2007]

## 2 Estrutura do Projeto
       A_quiz/
├── cadastro/                   # Módulo de cadastro de usuários
│   ├── bd.txt                  # Esboço/estrutura de banco de dados
│   ├── cadastro.php           # Página de cadastro
│   ├── db_quiz.mwb            # Modelo do banco de dados (MySQL Workbench)
│   ├── fro.jpg                # Imagem usada no projeto
│   ├── jin.jpg                # Imagem usada no projeto
│   ├── login.php             # Página de login
│   ├── processa_cadastro.php  # Script de processamento do cadastro
│
├── quiz/                      # Módulo com os níveis do quiz
│   ├── dificil.php            # Quiz nível difícil
│   ├── facil.css              # Estilo do quiz fácil
│   ├── facil.php              # Quiz nível fácil
│   ├── medio.php              # Quiz nível médio
│   ├── quiz.js                # Script JavaScript para funcionamento do quiz
│   ├── quizzes.sql            # Script SQL para tabela de quizzes
│
├── ranking/                   # Módulo de ranking
│   ├── db_quiz.tbl_usuario    # Estrutura da tabela de usuários
│   ├── processa_ranking.php   # Script para processar pontuações
│   ├── ranking.php            # Página que exibe o ranking
│
├── bd.txt                     # Esboço do banco principal
├── db_quiz (2).mwb            # Modelo alternativo do banco
├── db_quiz.mwb                # Modelo principal do banco de dados
├── estilo.css                 # Estilo geral do site
├── index.html                 # Página inicial do projeto
├── db_quiz.sql                # Script SQL para estrutura completa do banco
├── db_quizz.sql               # Versão alternativa do script SQL
├── documentação-testeS.pdf    # Documentação do projeto
├── model.mwb                  # Modelo adicional de banco de dados

## 3 Configuração do Ambiente ### **Requisitos**
    • Servidor XAMP
    • Visual Studio Code[1.98.2]
    • MySQL  Workbench[8.0.36]
    • Sistema operacinal: Windows 11;
    ### **Instalação**
    
1. Clone o repositório:
bash
git clone https://github.com/mimistudies90/Sistema-Quiz.git
cd 

 2. Instale as dependências:
 git,xamp


 3. Configure o banco de dados:
 Aqui está a versão estruturada e organizada do seu passo a passo para configurar o banco de dados MySQL:

4. Configure o banco de dados:
Coloque a senha do bd da sua maquina lócal na pasta 'cadastro.php','ranking.php'

5. Inicie o servidor:
http://localhost/


## 4 Estrutura do Banco de Dados ###

**Usuários (usuario)**
    • `id` (SMALLINT, PK, AUTO_INCREMENT)
    • `nome` (VARCHAR)
    • `email` (VARCHAR, UNIQUE)
    • `senha` (VARCHAR)
    
### **Ranking (ranking)**
    • `id` (SMALLINT, PK, AUTO_INCREMENT)
    • `pontuacao` (NOTNULL)
    • `tbl_usuario_usuario` (NOTNULL,FK)
  

### **Perguntas (perguntas)**
    • `id` (SMALLINT, PK, AUTO_INCREMENT,NOTNULL)
    • `pergunta` (VARCHAR)
  

### **Resposta_certa (resposta_certa)**
    • `id` (SMALLINT, PK, AUTO_INCREMENT,NOTNULL)
    • `resposta_certa` (NOTNULL)
    • `tbl_perguntas_id_perguntas` (SMALLINT)

    
### **Resposta_errda (resposta_errada)**
    • `id` (SMALLINT, PK, AUTO_INCREMENT,NOTNULL)
    • `resposta_errada` (NOTNULL)
    • `tbl_perguntas_id_perguntas` (SMALLINT)
    
    
    
   
