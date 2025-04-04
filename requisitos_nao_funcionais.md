# Requisitos Não Funcionais

## 1 - Objetivos Gerais:
### 1.1 - Esse documento lista os requisitos não funcionais que o sistema deve atender em relação ao seu funcionamento.
### 1.2 - O documento esta organizado em tópicos, esses tópicos são funcionalidades que o sistema irá implementar. Cada tópico será analisado tendo em vista esses três critérios: Restrição, Padrão de Qualidade e Critério Técnico.

## 2 - Escopo:
Tendo em vista o escopo do projeto, o mesmo deve atender aos seguintes requisitos:

| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
Não armazenará dados pessoais dos usuários | O tempo de resposta em todas as páginas do sistema não deve ultrapasar 5 segundos | O usuário deve navegar em todas as telas de forma simples e natural 
Não aceitará usuários sem identificação institucional | O sistema deve estar disponível para acesso as informações 24h por dia | O sistema deve ser fácil de usar e entender suas funcionalidades, de forma que o usuário não leve muito tempo em determinado recurso 
O produto só aceitará publicação de conteúdos relacionados ao contexto do sistema | Em relação aos dados, o sistema só armazenará o nescessário tendo em vista o desempenho do mesmo como também os dados devem ser armazenados de forma segura e confiável para passar confiabilidade aos usuários | Em relações as normativas de software, o sistema deve segui-las a risca de modo que o mesmo possa operar em produção de modo legal


## 3 - Problema de Falta de Informação aos Alunos
Um dos problemas que o sistema deve solucionar, é a questão da falta de informação para os alunos, o que gera desitência e evação universitária, na solução desse problea, o sistema deve atender o seguintes requisitos:
| Restrição | Critério Técnico | Padrão de Qualidade |
|-----------|------------------|---------------------|
| O sistema não informará notas curriculares dos alunos | Informações divulgadas devem estar disponiveis instantâneamente para os usuários em menos de 3 segundos | As informações devem ser apresentadas e visualizadas de forma simples, fácil e natural | 
| Vagas que já passaram do prazo de inscrição ou não são relacionadas a área de tecnologia, não serão divulgadas | O sistema deve carregar a listagem de vagas em menos de 2 segundos mesmo tendo muitos usuário logados simultâneamente  | Informações divulgadas devem ser analisadas para garantir que as mesmas são verdadeiras e integras |



| O que o sistema deve fazer                                                                                | O que ele faz | 
| --------------------------------------------------------------------------------------------------------- | ------------- |
| Operações como publicação/edição de vagas devem  ser processadas em **até 2 segundo**.                    | _             |
| O sistema deve carregar listagens de vagas em **menos de 2 segundos** mesmo com 500 usuários simultâneos. | -             |
| O produto deverá ter **alta disponibilidade**, por exemplo, 99% do tempo.                                 | -             |

## 5.2 Escalabilidade 
O produto não tem necessidade de ser escalável, ainda, haja visto que tem um objetivo claro, porém, em um sentido hipotético seria interessante:
- Integração com o **SIGAA** para saber se a matrícula ainda está ativa;
- O código deverá ser modular e documentado para facilitar atualizações futuras;

## 5.3 Segurança
| Recursos de Segurança                                   | Descrição                                                                                |
| ------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Validação de usuário                                    | Se faz necessária o uso do **e-mail institucional** em favor da segurança do produto.    |
| Dados sensíveis só são visíveis para **alunos logados** | O produto não deverá ser usável sem autenticação do aluno.                               |
| **Criptografia** dos dados para todas as comunicações.  | O produto não apresentará aos usuários quaisquer dados de cunho privativo.               |
| Acesso **restrito** por autenticação                    | O produto não deverá aceitar post de professores que não tiverem o e-mail institucional. |
| **Validação** de novos posts                            | Se faz necessária validação dos posts inseridos no produto.                              |

## 5.4 Usabilidade
A principio, o usuário deve navegar de forma **fácil e natural** entre as páginas do produto e da mesma forma o professor deverá ser capaz de **criar um novo post, editar e exclui-lo** de modo que não leve muito tempo para entender como usar, além de que O produto deverá ser responsiva a todos os ambientes.

## 5.5 Normativos/Legais
| Recursos Legais                    | Descrição                                                                       |
| ---------------------------------- | ------------------------------------------------------------------------------- |
| Está em sintonia com a instituição | O produto deverá seguir a política de estágio/extensão **proposta pela UESPI**. |
| **Backups** de logs                | Deverá haver um backup de dados sensíveis                                       |
## 5.6 Diferenciais
| Diferencial                 | Descrição                                                                                                           |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Integração com outras API´s | O produto deverá integrar com o site/e-mail do fornecedor da vaga/projeto de extensão, para o aluno ser encaminhado |
| -                           | -                                                                                                                   |
## 5.7 Tecnologias a serem usadas
| Tecnologia | O que faz                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------ |
| -          | A linguagem de programação há de ser discutida.                                                                          |
| -          | O produto deverá se comunicar com o SQL Server ou quaisquer banco de dados definido pelos administradores.               |
| -          | O padrão de infraestrutura e o método de organização ainda não foram discutidos (provavelmente MVC ou Cliente-Servidor). |