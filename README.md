# EventosApp-SpringBoot

Aplicativo simples em **Spring Boot**, desenvolvido com **Thymeleaf** para a renderização da interface e estilizado com **Materialize CSS**. Utiliza o **MySQL** como banco de dados, proporcionando um sistema para gerenciar eventos e seus respectivos convidados.

## Tecnologias Utilizadas

- **Spring Boot**
- **Thymeleaf**
- **Materialize CSS**
- **MySQL**

## Recursos

- Criar novos eventos com detalhes como nome, local, data e horário.
- Adicionar e remover convidados de eventos específicos.
- Ver uma lista de todos os eventos e seus detalhes.
- Excluir eventos juntamente com as informações de seus convidados associados.

## Passos Para Uso

1. Clone este repositório em sua máquina local.
2. Certifique-se de que você tenha o **MySQL** instalado e em execução.
3. Configure as configurações de conexão com o banco de dados no arquivo `application.properties`.
4. Compile e execute o aplicativo **Spring Boot** usando sua IDE preferida ou executando `mvn spring-boot:run` no terminal.
5. Acesse o aplicativo abrindo um navegador da web e navegando para `http://localhost:8080`.

## Uso

1. Crie um novo evento:
   - Acesse `/cadastrarEvento` e preencha os detalhes necessários.
   - Clique em "Salvar" para criar o evento.

2. Adicione convidados a um evento:
   - Após criar um evento, clique em seu nome na lista de eventos.
   - Adicione os detalhes do convidado no formulário fornecido e clique em "Adicionar".

3. Veja eventos e listas de convidados:
   - Acesse `/eventos` para ver a lista de todos os eventos.
   - Clique no nome de um evento para ver seus detalhes e lista de convidados.

4. Exclua eventos e convidados:
   - Para excluir um evento, clique no botão "Deletar" ao lado dos detalhes do evento.
   - Para excluir um convidado, clique no ícone "delete" ao lado dos detalhes do convidado.

## Observações

- Ao excluir um evento, todos os convidados associados aquele evento serão excluídos automaticamente no banco de dados. Essa funcionalidade pode ser alterada na linha 35 de Evento.java no pacote com.eventosapp.models.
