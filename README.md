# PJ_WEB
 Alunos: André Fellype e Yuri

O projeto esta em Estoque

# Sistema de Gerenciamento de Estoque

## Sobre o Projeto
Este projeto é um **Sistema de Gerenciamento de Estoque** desenvolvido em **Laravel**. Ele permite o cadastro, listagem, edição e exclusão de produtos, além de funcionalidades como autenticação de usuários e geração de relatórios.

## Tecnologias Utilizadas
- **PHP 8**
- **Laravel**
- **PostgreSQL**
- **Blade (Template Engine do Laravel)**
- **Bootstrap (SB Admin 2 Theme)**
- **JavaScript (jQuery e Chart.js)**

## Estrutura do Projeto
```
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   │   ├── EstoqueController.php
│   │   │   ├── AuthController.php
│   ├── Models/
│   │   ├── Produto.php
│
├── resources/
│   ├── views/
│   │   ├── layout/
│   │   ├── index.blade.php
│   │   ├── tables.blade.php
│   │   ├── cadastro_produto.blade.php
│   │   ├── edit_produto.blade.php
│
├── routes/
│   ├── web.php
│
├── public/
│   ├── css/
│   │   ├── sb-admin-2.min.css
│   ├── js/
│   │   ├── sb-admin-2.min.js
│
├── database/
│   ├── migrations/
│   │   ├── create_produtos_table.php
│
├── README.md
```

## Instalação e Configuração
1. Clone o repositório:
   ```bash
   git clone https://github.com/FellypeAndre/PJ_WEB.git
   cd Estoque
   ```
2. Instale as dependências:
   ```bash
   composer install
   ```
3. Copie o arquivo de configuração e gere a chave da aplicação:
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```
4. Configure o banco de dados no arquivo `.env`:
   ```
   DB_CONNECTION=pgsql
   DB_HOST=127.0.0.1
   DB_PORT=5432
   DB_DATABASE=ManuMaster
   DB_USERNAME=manumaster
   DB_PASSWORD=1234
   ```
5. Execute as migrações para criar as tabelas:
   ```bash
   php artisan migrate
   ```
6. Inicie o servidor:
   ```bash
   php artisan serve
   ```

## Funcionalidades
- [x] Cadastro de produtos
- [x] Listagem de produtos
- [x] Edição e exclusão de produtos
- [x] Autenticação de usuários
- [x] Dashboard com gráficos

## Telas do Sistema
### Tela de Cadastro de Produto
Permite adicionar novos produtos ao estoque com nome, descrição, preço e quantidade.

### Tela de Listagem (Tables)
Exibe todos os produtos cadastrados em uma tabela bem organizada.

### Dashboard
Página inicial do sistema, com gráficos e estatísticas sobre os produtos.

## Licença
Este projeto está sob a licença MIT - sinta-se à vontade para modificar e utilizar!

## Contato
📧 Email: andre.fellype39@gmail.com & yurisdepaula@gmail.com
🐙 GitHub: https://github.com/FellypeAndre & https://github.com/yuridpaula19
