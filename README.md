# Projeto Banco de Dados LINUX_DB

## Requisitos

Antes de começar, certifique-se de que os seguintes itens estão instalados no ambiente de desenvolvimento:

- **Node.js**: Necessário para executar os módulos `app-banco-de-dados` e `server-banco-de-dados`.  
  - [Baixar Node.js](https://nodejs.org)  
- **phpMyAdmin**: Utilizado para gerenciar e executar o script de criação do banco de dados.  
  - Consulte a documentação oficial para instalação no seu sistema.  

---

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

## Configuração da Conexão com o Banco de Dados

No módulo `server-banco-de-dados`, configure a conexão com o banco de dados ajustando o seguinte trecho de código no arquivo responsável pela conexão (server.js):

### Parâmetros da Conexão

- **`host`**: Define o endereço do servidor onde o banco de dados está hospedado. Para ambientes locais, utilize `"localhost"`.  
- **`user`**: Nome do usuário com permissão para acessar o banco de dados. Geralmente, para desenvolvimento, é `"root"`.  
- **`password`**: A senha do usuário do banco de dados. Deixe vazio `""` se não houver senha configurada.  
- **`database`**: O nome do banco de dados utilizado. No caso deste projeto, é `"linux_db"`.


```
const conexao = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "",
  database: "linux_db",
});

```

---

## Configuração do projeto

- Certifique-se de que o banco de dados `linux_db` está configurado corretamente.
- Verifique as credenciais do banco de dados no módulo `server-banco-de-dados`.
- Após configurar, inicie os módulos:
   - Para a Interface e Server execute :

  
     ```
     npm run dev
     ```

---

## Observação

Certifique-se de que o servidor MySQL esteja rodando corretamente e que a configuração do banco de dados no módulo server-banco-de-dados aponte para a base de dados linux_db criada no phpMyAdmin.


## Tutorial de Instalação


<iframe width="560" height="315" src="https://www.youtube.com/embed/Am3Ckwrkt7w?si=5y3TqnPfjOs6LcpJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



