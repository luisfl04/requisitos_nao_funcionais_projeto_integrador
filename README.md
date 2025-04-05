# Requisitos Não Funcionais

## 1 - Objetivos Gerais:
### 1.1 - Esse documento lista os requisitos não funcionais que o sistema deve atender em relação ao seu funcionamento.
### 1.2 - O documento esta organizado em tópicos, esses tópicos são funcionalidades que o sistema irá implementar. Cada tópico será analisado tendo em vista esses três critérios: Restrição, Padrão de Qualidade e Critério Técnico.

## 2 - Escopo:
Tendo em vista o escopo do projeto, o mesmo deve atender aos seguintes requisitos:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
Não armazenará dados pessoais dos usuários. | O tempo de resposta em todas as páginas do sistema não deve ultrapasar 5 segundos. | O usuário deve navegar em todas as telas de forma simples e natural. 
Não aceitará usuários sem identificação institucional. | O sistema deve estar disponível para acesso as informações 24h por dia. | O sistema deve ser fácil de usar e entender suas funcionalidades, de forma que o usuário não leve muito tempo em determinado recurso. 
O produto só aceitará publicação de conteúdos relacionados ao contexto do sistema. | Em relação aos dados, o sistema só armazenará o nescessário tendo em vista o desempenho do mesmo como também os dados devem ser armazenados de forma segura e confiável para passar confiabilidade aos usuários. | Em relações as normativas de software, o sistema deve segui-las a risca de modo que o mesmo possa operar em produção de modo legal.


## 3 - Problema de Falta de Informação aos Alunos
Um dos problemas que o sistema deve solucionar, é a questão da falta de informação para os alunos, o que gera desitência e evação universitária, na solução desse problea, o sistema deve atender o seguintes requisitos:
| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não informará notas curriculares dos alunos. | Informações divulgadas devem estar disponiveis instantâneamente para os usuários em menos de 3 segundos. | As informações devem ser apresentadas e visualizadas de forma simples, fácil e natural. | 
| Vagas que já passaram do prazo de inscrição ou não são relacionadas a área de tecnologia, não serão divulgadas. | O sistema deve carregar a listagem de vagas em menos de 2 segundos mesmo tendo muitos usuário logados simultâneamente.  | Informações divulgadas devem ser analisadas para garantir que as mesmas são verdadeiras e íntegras. |


## 4 - Divulgações de cursos de extensão
O sistema deve divulgar cursos de extesão relacionados a tecnologia, nessa funcionalidade, o mesmo deve seguir os seguintes requisitos:


| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O produto não deve dilvugar cursos que não sejam relacionados a área de tecnologia como também cursos que não ofereçam certificados após a conclusão.  | O sistema deve conseguir processar no mínimo 5 requisições de usuários em um mesmo segundo em relação a inscrição em cursos de extensão. | A inscrição em cursos de extensão no sistema deve ser feita de forma que o usuário mais leigo possível consiga se inscrever sem problemas e complicações.  |


## 5 - Eventos da Comunidade
Um dos requisitos é fazer com que o sistema consiga fazer a divulgação e inscrição de eventos relacionados a comunidade, em relação a essa funcionalidade, a mesma deve atender aos seguintes requisitos abaixo:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| Eventos presenciais, devem ser relacionados a eventos feitos e realizados no território do estado do Piauí. Eventos fora do estado só devem ser cadastrados se forem feitos de forma online. | Tendo em vista essa listagem de eventos, a mesma deve carregar em menos 2 segundos após a requisição da página feita pelo usuário. | A página de eventos deve listar os mesmos de forma rápida e fluída para os usuários.  |


## 6 - Vagas de Estágio e Emprego
Vagas de estágio e empregos que são elegíveis a usuários do sistema, devem ser divulgadas pelo mesmo, em relação a essa funcionalidade, o sistema deve garantir os seguintes requisitos:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
|O sistema não deve aceitar vagas que não estejam dentro do escopo da área de tecnologia. | Filtros realizados em relação a vagas, não devem demorar mais que 3 segundos para serem processados, como também as vagas devem ser renderizadas em mesmo tempo de processamento. | O usuário deve ser capaz de escolher entre qual área a vaga de emprego/estágio deve ser buscada e apresentada, em relação a essa funcionalidade, o sistema deve promover um sistema de navegação simples e otimizado, que faça com que o usuário navegue nessa página de forma rápida e natural, garantindo uma boa usabilidade. | 


## 7 - Informações cadastradas por Professores
Professores tem autonomia para cadastrar informações que serão visualizadas pelos alunos, dentre elas estão: divulgação de vagas de estágio, emprego, cursos de extensão e etc... Em relação a essa funcionalidade, a mesma deve atender as requisitos de qualidade abaixo:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não cadastrará informações relacionadas a conteúdos de disciplinas ministradas por professores. | Os posts cadastrados por professores não devem passar de 3 segundos para serem mostrados na tela após o cadastro dos mesmos. | Professores devem cadastrar e excluir suas divulgações sem complicações e contratempos. |


## 8 - Desempenho em navegadores web:
O sistema irá ser execultado em navegadores web, tendo em vista isso, ele deve atender aos seguintes requisitos de qualidade:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não funcionará em navegadores de versão antiga, tendo em vista que o mesmo será projetado para navegadores modernos que possuem mais suporte em relação as suas funcionlidades. | A cada 10 usuário logados simultâneamente, o sistema deverá ter uma margem de bug de no máximo 10%. Ou seja, a cada 10 usuários, será aceitável que bugs aconteçam em apenas 1 dos dispositivos. Essa é a margem total, no melhor caso, o sistema não deve apresentar bugs em nenhuma de suas instâncias. | A responsividade deve ser implementada em todas as telas, garantindo que o usuário consiga ter um mesmo padrão de navegação em todos os tamanhos de tela. |


## 9 - Perfis dos Usuários:
O produto abrange vários perfís de usuários, indo de usuário comuns(Alunos), até administradores. Em relação a essa funcionalidade, o mesmo deve atender aos seguintes requisitos:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não irá ter funcionalidade de autopromoção de perfil/privilégios do usuário, esse processo poderá ser feito unicamente por um administrador do sistema. | A atualização dos dados de perfil do usuário deve ser feita de forma instantânea, garantindo que os dados sejam atualizados em até 3 segundos tanto no banco de dados quanto na sua visualização por parte do usuário. | Em relação as telas que determinado tipo usuário pode visualizar, as mesmas devem estar disponíveis para acesso de forma instântanea e natural. Ainda sobre as telas, em relação as telas que não abrangem o tipo de usuário que está logado, essas mesmas telas não devem ser apresentadas, garantindo que cada tipo de usuário tenha um ambiente separado de acordo com seu perfil. |


## 10 - Capacidades de Uso de Acordo com o Tipo de Usuário
Como falado no tópico acima, cada usuário tem um tipo, e cada tipo tem as suas capaciades em relação a sua **interação** com o sistema, em relação a esses diferentes níveis de capacidade de interação, o sistema deve atender aos seguintes critérios de qualidade:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não verificará a exclusão de perfís comuns(Alunos e Professores), ou seja, usuários desses tipos poderão excluir suas contas a qualquer momento. | Mesmo tendo diferentes tipos de usuários interagindo ao mesmo tempo com o sistema em instâncias diferentes do mesmo, o sistema não deve ter seu desempenho degragado e deve garantir um tempo de resposta máximo de 3 segundos. | Tendo em vista que cada tipo de usuário possuirá uma interface personalizada em relação a página inicial, o sistema deve garantir que essa interface seja feita de forma que esteja atrelada ao tipo de usuário, proporcionando um experiência personalizada.|
