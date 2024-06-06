# Projeto Escola ACME

Este é um projeto desenvolvido para gerenciar informações de uma escola fictícia chamada Escola ACME. O objetivo principal é fornecer uma plataforma onde é possível gerenciar turmas,
professores e alunos de forma fácil e organizada. As tecnologias utilizadas incluem Pug, Node.js e Prisma.

## Funcionalidades Principais

- **CRUD**: O projeto inclui operações CRUD (Create, Read, Update, Delete) distribuídas entre as entidades Turmas, Professores e Alunos.

- **Renderização de Dados com Pug**: Utiliza-se o motor de template Pug para renderizar os dados dinâmicos nas páginas HTML. 

- **Modal para Cadastro de Turmas**: Implementa um modal que permite cadastrar uma nova turma.

- **Turmas**: No modal de detalhes da Turma, assim que um professor e um aluno são cadastrados em determinado curso, é exibido o RA e o nome do Aluno e Nome e Especialidade do Professor da Turma cadastrada.

- **Botão Novo Professor**: Simplifica o processo de adição de novos membros ao corpo docente da escola.

- **Cadastro de Professores**: Ainda dentro da tabela Professores em 'Acões', ao clicar em (' * '), abre-se um modal para alterar Professores. Nele é possível alterar o Nome, a Especialidade e a Turma que fica localizada em um seletor. 

- **Botão para Excluir Professores**: Foi acrescentado um botão para 'excluir professores' individualmente. Isso facilita a remoção de professores que não são mais necessários em determinada função.

- **Botão para Alterar dados do Aluno**: Na tabela de alunos, abre-se um modal onde são editados os dados de cada aluno e outro botão para excluir aluno com uma mensagem de alerta sobre a exclusão. Isso permite a atualização de informações pessoais conforme necessário.

## Tecnologias utilizadas

- **Pug**: Motor de template que simplifica a criação de interfaces HTML dinâmicas.

- **Node.js**: Ambiente de execução JavaScript que permite a construção de aplicativos de servidor escaláveis e eficientes.

- **Prisma**: ORM (Object-Relational Mapping) para banco de dados SQL, simplificando as operações de banco de dados e fornecendo uma interface fácil de usar para interagir com o banco de dados. 

- **XAMPP MySQL**: Conjunto de software gratuito e de código aberto que inclui Apache, MySQL, PHP e Perl. É usado para criar um ambiente de desenvolvimento local para sites dinâmicos.

## Como rodar o projeto

- Clone este repositório em sua máquina local.
- Abra com o VsCode.
- No terminal em cmd ou bash, instale as dependências:

```cmd
npm i
```
- Configure o arquivo .env com a string a seguir:

```cmd
DATABASE_URL="mysql://root@localhost:3306/escola?schema=public&timezone=UTC"
```

- Configure a conexão com o banco de dados no arquivo prisma/schema.prisma. Criar a migração, abrir o XAMPP, clicar em start no MySQL e Apache. No teminal do VsCode executar o comando:

```cmd
 npx prisma migrate dev --name init
```

 - Executar o Servidor para iniciar o servidor Node.js.

 ```cmd
 nodemon
 ```

 - Acesse a aplicação no navegador usando o endereço http://localhost:3000. 

## Print das Telas

- Tela Turmas

![tela turmas](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/521e89a1-6e0f-4650-974e-0ea723d49402)

- Modal Cadastro de Turmas
 
![modal turmas](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/c4a68f20-5ce3-4b68-9774-63c08eb9bbee)

- Modal Detalhes da Turma
 
![modal detalhes da turma](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/16269fa5-98c2-4ef0-9406-3a333d3ddd82)

- Modal Cadastro de Alunos

 ![modal alunos](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/5159f41e-10c1-4b6e-b527-281584bbc97c)

 - Modal Editar Aluno

 ![modal editar aluno](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/8a17bc4c-1e18-4c8a-9649-3c1cdcb81eae)

 - Modal Excluír Aluno

 ![mensagem exclusão aluno](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/57d6290d-8d97-4f4c-9500-39f2bb3faa2a)

 - Tela Professores

![tela professores](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/ba46d1c1-70f4-4c89-af3f-a902d3892c8e)

- Modal Cadastrar Professores

![modal professores](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/6d392ef9-0355-4850-bc8b-0967c92e7864)

- Modal Alterar Professor

![modal alterar professor](https://github.com/Carla-coder/Escola_Prisma_Pug/assets/128012862/c7044028-544c-4002-a128-c6ff8af65459)

## Autores

- [@octokatherine](https://www.github.com/Carla-coder)

## Instituição de Ensino

- Escola Senai unidade Jaguariúna - Curso Técnico em Desenvolvimento de Sistemas FullStack  Segundo Semestre (2024)

- Professor responsável pelo Projeto: Wellington Fabio https://github.com/wellifabio
