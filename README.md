
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




## Autores

- [@octokatherine](https://www.github.com/Carla-coder)


## Instituição de Ensino

- Escola Senai unidade Jaguariúna - Curso Técnico em Desenvolvimento de Sistemas FullStack  Segundo Semestre (2024)

- Professor responsável pelo Projeto: Wellington Fabio https://github.com/wellifabio