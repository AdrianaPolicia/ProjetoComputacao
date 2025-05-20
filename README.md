# ProjetoComputacao

**O que o Model, o Controller e o Enpoint fazem no projeto?**

Models: os models são responsáveis por representar os dados do site. Eles fazem a conexão com o banco de dados, definindo o formato dos daddos e contendo funções para deletar, atualizar, buscar e inserir.

Controller: os controllers são responsáveis por controlar o que acontece quando o usuário faz uma requisição ao site. Eles recebem a requisição, chamam os modes para buscar ou modificar um dados e mandam uma resposta de volta.

Endpoints: os endpoints são os endereços (URL) que o navegador ou o sistema acessa para interagir com o site. Eles são as rotas do site, como alunos e professores.

**Como o Model, o Controller e a View interagem entre si?**

O Model, o Controller e o View trabalham em conjunto para organizar a lógica da aplicação de forma separada e eficiente. O Controller atua como intermediário entre o usuário e o sistema, o Model é responsável por acessar e manipular as informações do banco de dados e o View é uma página HTML com todos os dados que o Controller decidiu que será retornado ao usuário.

**Como ocorre o envio e o recebimento de dados no formato JSON neste projeto?**

O envio e o recebimento de dados em formato JSON neste projeto ocorrem principalmente nas rotas que servem como API. Assim, quando o usuário realiza uma ação que exige comunicação com o servidor sem recarregar a página, os dados são enviados ao servidor no corpo da requisição HTTP em formato JSON. O Controller recebe os dados, interage com o Model para realizar a operação necessária no banco de dados e responde com um objeto JSON contendo o resultado da operação. Essa troca permite que a interface do usuário seja atualizada. 
Um exemplo de rota que responde em JSON neste projeto pode ser encontrado no arquivo cursos.js na pasta routes. Essa rota é ativada quando o navegador ou uma aplicação cliente faz uma requisição. O controller responsável por essa rota chama o método para buscar todos os registros de cursos no banco de dados. Após obter os dados, ele envia a resposta para o cliente no formato JSON. 

**Qual a importância de usar HTML básico com formulários e tabelas para organizar e manipular dados no navegador?**

O uso de HTML básico com formulários e tabelas é importante em projetos back-end porque oferece uma maneira simples, eficiente e acessível de interagir com dados diretamente pelo navegador, sem depender de frameworks front-end complexos. Formulários permitem a entrada estruturada de informações pelo usuário, enquanto as tabelas organizam visualmente os dados, facilitando a leitura, edição e exclusão de registros.