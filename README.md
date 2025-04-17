# Documento de visão

## Rede Social (IFormandos)

### Histórico da Revisão 

|  Data  | Versão | Descrição | Autores |
|:-------|:-------|:----------|:------|
| 13/03/2024 |  **`1`** | Início do documento de visão do projeto  | Beatriz Maria, Cauã Henrique, Matheus dos Santos, Sâmia Fernandes e João Vinícius.|
| 03/04/2024 |  **`2`** | Detalhamento dos requisitos funcionais do projeto  | Beatriz Maria, Cauã Henrique, Matheus dos Santos, Sâmia Fernandes, Izabel Alice, Lucas Albuquerque, João Vinícius, Kilton Jhonathan, Murillo Viniz e Rodrigo de Oliveira.|
| 03/04/2024 |  **`3`** | Atualizações com a exclusão do aluno representante | Rodrigo de Oliveira.|
| 01/02/2025 |  **`4`** | Adição dos novos RFs | Matheus dos Santos e Rodrigo de Oliveira.|
| 02/02/2025 |  **`4`** | Ajuste de RF's | Lucas Albuquerque |


### 1. Objetivo do Projeto 

O projeto __IFormandos__ tem como objetivo armazenar e exibir as placas das novas turmas formadas no IFRN campus Natal-Central (CNAT), para acabar com o problema da falta de espaço das paredes das diretorias.
 

### 2. Descrição do problema 

|         __        | __   |
|:------------------|:-----|
| **_O problema_**    | A falta de espaço nas paredes das diretorias para a instalação de novas placas de formatura.   |
| **_afetando_**      | Servidores das diretorias e alunos. |
| **_cujo impacto é_**| Causa a decepção por parte dos novos formandos, pois não podem colocar placas novas pela falta de espaço, bem como podem causar poluição visual se as placas continuarem a ser colocadas no espaço das diretorias.|
| **_Uma boa solução seria_** | Criar um sistema onde as novas placas seriam armazenadas e mostradas virtualmente, não sendo necessário conseguir mais espaço fisíco para elas e dando a todas as turmas a oportunidade de ter uma placa, pois há turmas que querem uma, porém não possuem a condição financeira para produzi-la.|


### 3. Descrição dos usuários

| Nome | Descrição | Responsabilidades |
|:---  |:--- |:--- |
| Alunos e ex-alunos do IFRN CNAT  | Frequentantes do IFRN e alunos egressos, que não possuem disponibilidade ou interesse em se deslocar até a instituição para ver sua placa. | Logar e deslogar na conta para acessar a comunidade; Visualizar placas; Fazer postagens na turma; Curtir, favoritar e comentar nas placas; Pôr uma descrição em seu perfil, que ficará público na aba da turma;|
| Visitante  | Usuário externo não cadastrado como membro da instituição. | Acessar o site; Pesquisar turmas e placas.|
| Administrador | A própria instituição. | Postar as placas no sistema; Desligar membros; Gerenciar as postagens; Gerenciar denúncias.|

### 4. Descrição do ambiente dos usuários

As postagens podem ser feitas a qualquer horário, com o sistema tendo a capacidade de receber postagens 24 horas por dia, nos 7 dias da semana. Porém, as postagens só são realmente enviadas para serem aprovadas se o usuário aluno/egresso estiver conectado à internet.
Os ex-alunos, alunos e os visitantes não possuem ambientes fixos para acessar o site, sendo necessário apenas uma conexão com a internet para que isso seja feito.
O administrador já possui uma gama menor de locais para acessar o site, necessitando de uma conexão estável com a internet e sendo muito provável que ele acesse o site de um computador dentro da instituição ou de um computador específico para trabalho.


### 5. Principais necessidades dos usuários
As pessoas que frequentam, ou já frequentaram, o CNAT percebem que cada vez mais as paredes das diretorias estão ficando sem espaço para colocar novas placas de formandos. Outro fato é que várias pessoas que fizeram placas de formando não querem ter que se deslocar para o CNAT para conseguir visualizar a sua placa, pois elas têm suas vidas e compromissos diários (como trabalho e estudos) a serem realizados.

A partir das informações acima seria interessante a existência de um site onde os usuários podem cadastrar placas de formatura para que as pessoas possam visualizá-las, e assim as placas estariam em exposição para as pessoas sem que houvesse a necessidade de colocá-las nas paredes.

Os usuários desejam poder manter contato com seus antigos colegas de turma que estão cadastrados no site e também interagir nas postagens de outras pessoas.


### 6.	Alternativas concorrentes
Como alternativas concorrentes podemos colocar redes sociais (ex: Instagram e etc) e também sites que permitem a visualização de placas de formandos.

Instagram:
Pontos fortes: A sua estrutura permite uma visualização boa das postagens das pessoas que você está seguindo.
Pontos fracos: Não permite somente a visualização das postagens de forma mais exclusiva ou visualização dos usuários, te mostrando diversos outros conteúdos.

Parte do site da UniFacema que permite a visualização das placas:
Pontos fortes: É um dos poucos sites que tem essa proposta.
Pontos fracos: Existem erros de design que podem gerar desconforto visual durante a navegação.



### 7.	Visão geral do produto
A rede social em desenvolvimento deve ser feita para ser utilizada em navegadores (browsers);
Será possível vincular seu email escolar e sua matrícula ao site. (ainda em análise)  
O site tem 4 tipos de usuário. O usuário visitante, quando não é cadastrado, pode acessar o site e pesquisar por placas de seu interesse, mas não pode comentar, curtir e favoritar as publicações. 
O aluno/ex-aluno seria um usuário cadastrado, podendo interagir com as placas, entrar em sua turma, ter um perfil próprio, fazer postagens, dar likes, favoritar e fazer comentários.
O administrador será um moderador do sistema, não necessariamente usufruindo desse.
 

### 8. Requisitos Funcionais

| Código | Nome | Descrição |
|:---  |:--- |:--- |
| RF01 | Fazer o login de usuário | Para fazer o primeiro login o usuário precisará preencher um campo formulário com sua matrícula ou e-mail escolar e senha. Os logins seguintes poderão ser feitos inserindo a matrícula e o e-mail escolar ou, se o usuários tiverem cadastrado um e-mail pessoal na sua conta, ele poderá ser usado para o login e insertando a senha. Logo após o login, o usuário será redirecionado para a página inicial do site. |
| RF02 | Realizar buscas | Os usuários em geral terão acesso à área de pesquisa do sistema para encontrar algo em específico. Nessa área, na página home, eles poderão pesquisar por uma placa. Eles terão suporte de filtros contendo um local onde poderão colocar o nome da turma, um local para escolher o curso e um local para colocar o ano de conclusão. Além disso, na página de explorar, os usuários poderão pesquisar por postagens e alunos específicos. |
| RF03 | Interagir com publicações |  Os usuários aluno e ex-aluno de turma poderão curtir, comentar, deunuciar e salvar/favoritar uma postagem, além de denunciar um comentário. O usuário visitante não poderá interagir com as postagens e placas, apenas visualizá-las. O usuário administrador irá fiscalizar as postagens e os comentários, podendo apagá-los, bem como as denuncias, as quais podem ser visualizadas e solunionadas. Todos os usuários poderão denunciar uma postagem e/ou comentário, cabendo ao administrador averiguar a necessidade de excluir esses. Todos os usuários poderão visualizar a página de turmas. |
| RF04 | Gerenciar turmas | O usuário administrador poderá criar uma turma e, a partir disso, os componentes a ela de forma automatizada ou manual, caso seja necessário. Para tanto, a adição dos membros, sejam professores ou alunos, será realizada por dados obtidos via SUAP. O usuário administrador também poderá editar a turma criada, caso necessário. |
| RF05 | Gerenciar postagem do próprio usuário | Os usuários aluno e ex-aluno poderão fazer, editar e excluir postagens. Para a criação de postagens, os usuários têm a capacidade de inserir texto, imagens, vídeos e outros tipos de mídia. A edição de postagens permite aos usuários modificar o conteúdo, adicionar ou remover mídias e atualizar informações relacionadas, com as alterações refletidas instantaneamente após a confirmação. A exclusão de postagens está disponível a qualquer momento, com a solicitação de uma confirmação para evitar exclusões acidentais, e todas as interações associadas, como curtidas e comentários, são removidas do sistema. |
| RF06 | Gerenciar placas | O usuário administrador poderá criar uma placa e, a partir disso, os componentes e orientadores da placa serão adicionados a ela de forma automatizada ou manual, caso seja necessário. Para tanto, a adição dos membros, sejam professores ou alunos, será realizada por dados obtidos via SUAP. |
| RF07 | Gerenciar perfil | O usuário e/ou visitante pode compartilhar o perfil de um usuário. O sistema deve oferecer múltiplas opções para compartilhar o perfil do usuário, incluindo compartilhamento por meio de links permanentes, como redes sociais, whatsapp, discord e entre outros canais relevantes. |
| RF08 | Suspender aluno | O usuário administrador pode suspender um usuário aluno/ex-aluno caso julgue necessário, a partir de comportamentos inadequados do último. A duração da suspensão dependerá da gravidade do ato do usuário que o cometeu, ficando ele impossibilitado de fazer uso das funções do sistema. |
| RF09 | Criar usuário | O usuário administrador pode gerar os usuários servidor e aluno no sistema quando necessário. Somente após isso, os usuários servidor e aluno poderão utilizar as funções do sistema de forma plena. |
| RF10 | Criar curso | O usuário administrador pode criar um curso no sistema conforme achar necessário. Toda turma deve estar associada a um curso. |


### 9. Requisitos não-funcionais

 Código | Nome | Descrição | Categoria | Classificação
|:---  |:--- |:--- |:--- |:--- |
| RNF01 | Design responsivo | O sistema deve adaptar-se a qualquer tamanho de tela de dispositivo, seja, computador, tablets ou smart phones. | Usabilidade | Opcional |
| RNF02 | Privacidade | O sistema não deve revelar informações pessoais sobre seus usuários | Segurança | Obrigatório |
| RNF03 | Facilidade de uso | O sistema deve ter uma interface de fácil entendimento | Usabilidade | Obrigatório |
| RNF04 | Acesso inclusivo | Ser acessível para todos os usuários, independentemente de suas habilidades | Acessibilidade | Obrigatório |
| RNF05 | Criptografia de dados| Os dados devem ser gravados de forma criptografada no banco de dados | Segurança | Obrigatório |

