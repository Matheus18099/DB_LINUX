# Projeto Banco de Dados

## Descrição

Este projeto é composto por dois módulos principais: 

- **`app-banco-de-dados`**: Interface do aplicativo.  
- **`server-banco-de-dados`**: Servidor responsável pela comunicação com o banco de dados.  

Além disso, há um arquivo chamado **`SCRIPT_BANCO_DE_DADOS`**, que contém o script necessário para a criação da estrutura do banco de dados.

---

## Instalação

1. **Baixar os arquivos**
   - Faça o download das pastas `app-banco-de-dados` e `server-banco-de-dados`, além do arquivo `SCRIPT_BANCO_DE_DADOS`.

2. **Instalar as dependências**
   - Navegue para cada uma das pastas (`app-banco-de-dados` e `server-banco-de-dados`).
   - Abra o terminal em cada pasta e execute o seguinte comando:
     ```
     npm install
     ```
   - Este comando instalará todas as dependências necessárias.

3. **Criar o banco de dados**
   - Abra o arquivo `SCRIPT_BANCO_DE_DADOS`.
   - Copie todo o conteúdo do arquivo.
   - Acesse o **phpMyAdmin**.
   - No phpMyAdmin, crie um banco de dados chamado **`linux_db`**.
   - Na interface SQL do phpMyAdmin, cole o conteúdo do arquivo copiado e execute o script.

---

## Configuração do projeto

- Certifique-se de que o banco de dados `linux_db` está configurado corretamente.
- Verifique as credenciais do banco de dados no módulo `server-banco-de-dados`.
- Após configurar, inicie os módulos conforme necessário (ex.: `npm start`).

---

## Observação

Certifique-se de que o servidor MySQL esteja em execução antes de iniciar o projeto.
"""
