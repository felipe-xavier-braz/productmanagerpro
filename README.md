# Sistema de Gerenciamento de Produtos

Este é um sistema para gerenciamento de produtos, desenvolvido com Laravel no backend e React no frontend. O sistema oferece funcionalidades para listar, adicionar, editar e excluir produtos, além de consumir uma API que retorna informações detalhadas de produtos. O Laravel Breeze foi utilizado para autenticação, e a interface responsiva foi construída utilizando React.

---

## Tecnologias Utilizadas

- **Laravel**: Framework PHP para construção do backend e da API RESTful.
- **Laravel Breeze**: Implementação de autenticação simples para registro, login e logout.
- **React**: Biblioteca JavaScript para a criação de uma interface de usuário dinâmica.
- **MySQL**: Banco de dados utilizado para armazenamento de informações.
- **Inertia.js**: Permite integração perfeita entre Laravel e React para a criação de SPAs.
- **Tailwind CSS**: Framework CSS para o design responsivo e estilizado da interface.
- **SweetAlert2**: Biblioteca JavaScript para exibir alertas e notificações modais elegantes.
- **Bootstrap**: Framework CSS para estilização e estruturação responsiva da interface.

---

## Funcionalidades Principais

### Backend
- **API RESTful**:
  - Endpoint de retorno de produto:
    ```json
    {
        "id": 47,
        "name": "LG C1 OLED",
        "description": "55-inch OLED Smart TV",
        "price": "1399.99",
        "quantity": 7,
        "active": true
    }
    ```
  - Suporte a operações CRUD (criação, leitura, atualização e exclusão) de produtos.
- **Autenticação**:  - Implementada com Laravel Breeze para registro, login e logout.

### Frontend
- **CRUD de Produtos**:  - Funcionalidades para listar, adicionar, editar e excluir produtos.
- **Paginação**:  - Componente de paginação dinâmica para navegar entre páginas de produtos.
- **Interface Responsiva**:  - Desenvolvida com React e estilizada com Tailwind CSS.
- **Status do Produto**:  - Campo de status ativo/inativo (ativo = 1, inativo = 0) com alternância simples.
- **Alertas e Validação**:  - Mensagens claras de sucesso e erro para feedback ao usuário.

---

## Configuração do Banco de Dados

    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=product_manager
    DB_USERNAME=root
    DB_PASSWORD=

## Instruções de Instalação e Execução

### Requisitos
- **PHP**: >= 8.0
- **Composer**: Para gerenciar as dependências do Laravel.
- **Node.js e npm**: Para o frontend React.
- **MySQL**: Banco de dados configurado e acessível.

### Passos
1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/felipexavier26/productmanagerpro.git
   cd seu-repositorio

2. **Configuração do Backend**:
   ```bash

   - Instale as dependências do Laravel
   composer install

   - Copie o arquivo de exemplo de configuração
   cp .env.example .env


3. **Execute as migrações e seeders**:
   ```bash
    php artisan migrate --seed

4. **Geração de Chave da Aplicação**:
   ```bash
    php artisan key:generate


5. **Configuração do Frontend**:
    ```bash
    - Instale as dependências do npm:
        npm install
    
    - Compile os arquivos do frontend
        npm run dev


6. **Inicie o Servidor de Desenvolviment**:
    ```bash
    php artisan serve

7. **Inicie o Servidor de Desenvolviment**:
    ```bash
    Abra o navegador em http://localhost:8000.
