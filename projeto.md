<img src='/img/NewLogo.png' alt='logo da empresa' width='100px' heidth='100px'/>

# *Run Noob*

# João

# PROJETO DE SOFTWARE

## *Stakeholders*
|NOME|CARGO|E-MAIL|
|:---|:---|:---|
|João Vitor Pereira Gomes|Gerente de Projeto e Programador|jvpg789@hotmail.com|
|Marcos Vinicius Dutra Lencina|Gerente de Configuração|marcosdutravini8@gmail.com|
|Suellen Thais Martin de Oliveira|Cordenador de Projeto|suellenthaisoliveira@gmail.com|
|Edmara Santos Cordeiro da Silva|Designer de Interface com o Usuário|edmarasantos1205@gmail.com|
|Tarcisio Santhiago Batista De Morais|Analista de Teste|tarcisiosantiago07@gmail.com|
|Karoline de Souza Cerozini|Analista de Requisitos|karolinecerozini15@gmail.com|


# Sumário

* [RESUMO DO PROJETO](#resumo-do-projeto)
* [INTRODUÇÃO](#introdução)
  * [PROPÓSITO DESTE DOCUMENTO](#propósito-deste-documento)
  * [ESCOPO DO PROJETO](#escopo-do-projeto)
  * [CONCEPÇÃO DO SISTEMA](#concepção-do-sistema)
  * [CONVENÇÕES, TERMOS E ABRIVEAÇÕES](#convenções-termos-e-abreviações)
* [DESCRIÇÃO GERAL](#descrição-geral)
  * [USUÁRIOS DO SISTEMA](#usuários-do-sistema)
  * [ABRANGÊNCIA E SISTEMAS SIMILARES](#abrangência-e-sistemas-similares)
  * [SUPOSIÇÕES E DEPENDÊNCIAS](#suposições-e-dependências)
* [ESTUDO DE VIABILIDADE](#estudo-de-viabilidade)
  * [VIABILIDADE TÉCNICA](#viabilidade-técnica)
  * [VIABILIDADE ECONÔMICA](#viabilidade-econômica)
  * [VIABILIDADE ORGANIZACIONAL](#viabilidade-organizacional)
* [METODOLOGIA ADOTADA NO DESENVOLVIMENTO](#metodologia-adotada-no-desenvolvimento)
* [REQUISITOS DO SOFTWARE](#requisitos-do-software)
  * [REQUISITOS FUNCIONAIS](#requisitos-funcionais)
  * [REQUISITOS NÃO FUNCIONAIS](#requisitos-não-funcionais)
* [PROTOTIPAGEM](#prototipagem)
* [DIAGRAMA DE CASOS DE USO](#diagrama-de-casos-de-uso)
  * [ESPECIFICAÇÃO DOS CASOS DE USO](#descrição--especificação-dos-casos-de-uso)
* [DIAGRAMA DE CLASSES](#diagrama-de-classes)
* [DIAGRAMA DE SEQUÊNCIAS](#diagrama-de-sequências)
* [ DIAGRAMA DE ATIVIDADES](#diagrama-de-atividades)
* [REFERÊNCIAS](#referências)


# RESUMO DO PROJETO
| ITEM | DESCRIÇÃO|
|:---|:---|
| NOME DO PROJETO | Run Noob |
| GERENTE DO PROJETO | João V. Pereira |
| PRINCIPAL OBJETIVO | Site e sistema de jogo com foco nos recordes obtidos |
| BENEFÍCIOS ESPERADOS | Forma de entreterimento superior |
| INÍCIO E TÉRMINO PREVISTOS | 14/03/2023 - 07/12/2023 |

[ [INÍCIO](#fibonacci-management-system) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_Run Noob_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema. O documento apresentará a ideia essencial da base principal da sistema.

## CONCEPÇÃO DO SISTEMA

Foram usados três métodos para que pudessem ser obtidos os requisitos do sistema:
* Entrevista:
  * Foram feitas entrevistas com clientes, e futuros usuários para se compreender o que é necessário para um bom sistema.
* Consulta com especialista:
  * Wagner da Silva, professor de Fundamentos em Análise de Sistemas no Instituto Federal orientou na concepção do sistema devido sua experiência em trabalhar em sistemas e ser um dos consultores da empresa;
  * Marco Andrade, professor de Análise e Desenvolvimento de Sistemas do Instituto  Federal orientou na análise de requisitos devido a sua grande experiência em desenvolvimento de software educativo;
* Prototipação:
  * Representações das interfaces gráficas feitas no figma e com diferentes níveis de fidelidade, aprovadas pela empresa contratante.



## CONVENÇÕES, TERMOS E ABREVIAÇÕES

Para evitar interpretações incorretas deste documento, algumas convenções e termos específicos são descritos a seguir:

* Noob: Iniciante em um jogo
* Level: nível, no contexto do sistema, nível de jogo
* Levels: níveis, no contexto do sistema, níveis do jogo

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## ESCOPO DO PROJETO

### NO ESCOPO

Run Noob é um jogo com uma coletânea  de fases onde o seu objetivo de cada uma delas é ser o mais rápido, cada fase está ligada a um placar, onde obviamente, quem é o mais rápido fica em primeiro. Competindo com os amigos e estranhos sempre tentando ser o mais rápido nesse jogo extremamente desafiante. Você é Noob, um carinha com o objetivo de ser o mais rápido deste planeta, e atingir esse objetivo definitivamente não vai ser fácil.
O escopo do **produto** pode ser consultado nos [requisitos do software](#requisitos-do-software)

### FORA DO ESCOPO

Não fazem parte do escopo do projeto:
* Instalação e configuração do ambiente tecnológico do cliente;
* Treinamento de instalação, configuração, administração e  utilização do sistema;
* Integração com quaisquer sistemas ou base de dados do ambiente tecnológico do cliente.

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Cadastrados:**|Usuários que cadastraram podem realizar ações, tal como:jogar e armazenar resultados da pertida, configurar perfil, analisar recordes passados, resultados de partidas recentes e analisar recorde de outros usuarios.|
|**Usuário Convidado:**|Usuários que não se cadastraram, por isso podem realizar menos ações , tal como: jogar, analisar resultados de partidas recentes e analisar recorde de outros usuários|
|**Administrador:**|Responsáveis pelo gerenciamento dos usuarios, levels, e recordes  dos usuários|


## Abrangência e sistemas similares

### Abrangência:

O sistema será um site web onde apresentará um gama de levels de um jogo plataformer, a unica mudançã de level para level será a mudança do cenário e os desafios presentes no level. A jogabilidade do jogo terá uma curva de aprendizado e sempre haverá uma margem para melhora e otimização para cada level. O objetivo do jogo é conseguir o menor tempo possível para completar um level, superando os próprios recordes e competindo para superar os recordes de outros ususários. No sistema haverá uma maneira de cadastrar um ususário para que possa salvar os recordes, e outros usuarios possam visualizar esses recordes. 

Das ferramentas de recordes e tempo podemos citar:

* **Analisar tempos recentes:** será possível comparar e analisar recordes recentes;

* **Analisar recordes de outros usuários:** será possível comparar e analisar recordes de outros usuários;

* **Comparar recordes antigos:** será possível comparar e analisar recordes antigos;

### Sistemas similares:

No cenário atual de sites de jogos web, existe inúmeros sites que apresentam uma biblioteca de jogos, entretanto, não existe um site no qual aplica esse conceito de jogos e recordes.

No cenário de sites de biblioteca de jogos web encontram-se três sistemas que se destacam:

**Friv:** é um site no qual apresenta uma biblioteca de jogos web com determinado estilo visual.

**Ojogos:** é um site brasilero, no qual apresenta um biblioteca de jogos, cadastramento de ususarios, avaliação de jogos e outras ferramentas.

**Poki:** é um site que tem uma biblioteca de jogos web, no qual tem uma vasta diversidade de jogos interativos com o foco principal nos infatis.

## Suposições e dependências
O sistema necessita de um servidor web para sua hospedagem e um servidor de banco de dados para o armazenamento das informações.

Os usuários devem utilizar navegador web Chrome, Firefox ou Safari com a seguinte configuração mínima:

* WebGL 1.0 ou 2.0
* HTML 5
* 64-bit
* WebAssembly

# ESTUDO DE VIABILIDADE

Uma vez definidos a necessidade para o sistema e seus requisitos de negócio, é possível compreender melhor o projeto do sistema proposto para elaborar o estudo de viabilidade com os seguintes destaques:

## Viabilidade Técnica
Os colaboradores da empresa contratante possuem bastante experiência com aplicações desta natureza, os analistas também estão familiarizados com esta área de aplicação comercial, porém o sistema utiliza uma tecnologia nova, com a qual os analistas e programadores não estão familiarizados. No que se refere ao tamanho do sistema, trata-se de um projeto de médio porte, com baixo nível de complexidade, que não será integrado a outros sistemas, limitando-se a atender a demanda da escola no que se refere à EaD, que, atualmente possui 1.000 alunos matriculados. Conclui-se que o projeto possui viabilidade técnica, em virtude dos baixos riscos identificados.

## Viabilidade Econômica

Foi realizada uma análise de custo-benefício, e, mesmo com estimativas conservadoras do retorno sobre o investimento e dos benefícios totais, este projeto é viável economicamente. Após a implantação, espera-se uma melhoria na qualidade dos serviços prestados e aumento da capacidade de vagas da unidade escolar.

## Viabilidade Organizacional

Do ponto de vista organizacional, este projeto apresenta baixo risco. Os diretores e coordenadores da instituição demonstram forte interesse no projeto. Espera-se que os professores e alunos aprovem a implantação do sistema, visto que atualmente a escola não possui uma ferramenta específica para o controle das informações, o que está provocando enormes transtornos para a instituição.


[ [INÍCIO](#fibonacci-management-system) ]

# Metodologia Adotada no Desenvolvimento


[ [INÍCIO](#fibonacci-management-system) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

## Requisitos Funcionais

A tabela a seguir contém a relação dos Requisitos Funcionais elicitados, com as colunas: identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
:---|:---|:---|
|RF-001 |Cadastrar usuários | O sistema permitirá que usuários sejam cadastrados, classificando eles como comum ou administrador |
|RF-002 |Entrar em uma conta | O sistema permitirá entrar em uma conta de um usuário cadastrado |
|RF-003 |Armazenar informações do jogo por usuário | O sistema armazenará as informações dos recordes do usuário por level  |
|RF-004 |Armazenar informações do perfil do usuário | O sistema armazenará as informações que aparecerá no perfil do usuário |
|RF-005 |Ordenar usuários por recordes| O sistema permitirá ver uma listagem dos usuários organizada pelo seus recordes adquiridos |
|RF-006 |Ordenar recordes em leveis| O sistema permitirá ver uma listagem de recordes por level baseada nos recordes atingidos  |
|RF-007 |Pesquisar por perfil de usuários | O sistema permitirá pesquisar por perfil de usuários |
|RF-008 |Visualizar perfil de usuário | O sistema permitirá visualizar o perfil de um usuário, assim mostrando suas informações de perfil e recordes |
|RF-009 |Contabilizar níveis de experiências do usuário| O sistema contabilizará níveis de experiência baseado nos recordes e outros fatores |
|RF-010 |Ordenar usuários por níveis de experiência | O sistema permitirá visualização de uma listagem de usuários ordenada por níveis de experiência  |
|RF-011 |Personalizar perfil de usuário | O sistema permitirá a personalização do próprio perfil de usuário |
|RF-012 |Excluir usuário | O sistema permitirá a exclusão do próprio perfil e usuário do sistema  |
|RF-013 |Jogar no site | O sistema permitirá que os usuários joguem o jogo no site do sistema para alcançar recordes|
|RF-014 | Histórico de recordes por usuário | O sistema permitirá a visualização de recordes obtidos por usuário |
|RF-015 |Histórico de recordes por level | O sistema permitirá a visualização de recordes por level |
|RF-016 |Administrar usuários | O sistema permitirá que os administradores administrem os usuários e perfis |
|RF-017 |Administrar recordes| O sistema permitirá que os administradores administrem os recordes alcançados por outros usuários |
|RF-018 |Filtrar informações de perfil | O sistema filtrará as informações do perfil de um usuário a fim e de evitar informações improprias |
|RF-019 |Ordenar perfis por país | O sistema permitirá uma visualização dos perfis de determinado país |
|RF-020 |Ordenar recordes por país | O sistema permitirá uma visualização dos recordes de  perfis de determinado país |


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001 |Taxa de atualização padronizada |A taxa de atualização durante o jogo para padronizar o jogo independente da maquina que está rodando  |
|RNF-002 | É preciso ter devido cuidado com os dados do usuário | O manejamento de dados deve seguir Lei Geral de Proteção de Dados Pessoais |
|RNF-003 | A equipe deve utilizar uma metodologia ágil | Para o desenvolvimento deve ser utilizado a metodologia ágil de Feature Driven Development em conjunto do Kanban |
|RNF-004 |Uso do Banco de Dados com MySQL | Os dados dos usuários e de recordes deverão ser armazenados no banco de dados com MySQL |
|RNF-005 | Será utilizado a framework Next.JS | Deverá ser utilizado a framework Next.Js e React.js para o desenvolvimento do sistema|
|RNF-006 | O desenvolvimento será baseado em componentização| O desenvolvimento do front-end do site será baseado em componentes feitos com React.js |
|RNF-007 | A linguagem utilizada no desenvolvimento será typescript | O desenvolvimento do sistema será feito em typescript |
|RNF-008 | Manejamento de versões com git e GitLab | O manejamento das versões do sistema será feito com git, as armazenando em um GitLab privado |
|RNF-009 | Responsividade para telas de desktops diferentes | O site deve ter responsividade para as diferentes telas de desktop |
|RNF-010 | O sistema deve ter compatibilidade com os navegadores | O site deve ter compatibilidade com os principais navegadores, ex: Google Chrome, Mozilla Firefox, Opera, Microsoft Edge,etc |


[ [INÍCIO](#fibonacci-management-system) ]


# Prototipagem

[Protótipo criado no FIGMA em 2022 por estudantes](https://www.figma.com/file/iNC7wyX9zP7Kmn3BhiCFGf/Fals6Hood-(Prot%C3%B3tipo-criado-por-estudantes-em-2022)?node-id=0%3A1&t=B16hgeZP3MSURCCa-1)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#fibonacci-management-system) ]


# Diagrama de Casos de Uso


![Diagrama de Casos de Uso](/img/use_case_placas.png)

## Descrição / Especificação dos Casos de Uso

### UC-01 - Cadastrar Professor

|UC-01 - Cadastrar Professor|           
|:---|
|**Descrição/Objetivo:** Permite a inclusão de novos professores no Sistema|
|**Atores: Administrador**|
|**Pré-condições:** O usuário precisa estar cadastrado e logado|
|**Pós-condições:** Será apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXO PRINCIPAL / BÁSICO:**|
|1. O usuário seleciona a opção cadastrar professor|
|2. Os dados do professor são inseridos|
|3. O usuário clica em salvar|
|4. Um novo ID é gerado |
|5. É apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXOS ALTERNATIVOS / EXCESSÕES:** |
|**A1: Campo obrigatório não preenchido** |
|1. Uma mensagem será apresentada para o usuário, informando que existe(m) campos obrigatórios que não foram preenchidos |
|2. O cursor será posicionado no primeiro campo obrigatório que não foi preenchido |
|**A2: Data de nascimento inválida** |
|1. Uma mensagem será apresentada para o usuário, informando que a data informáda não é válida|
|2. O cursor será posicionado para o campo data|


## Matriz de Rastreabilidade


| REQUISITO |UC-01|UC-02|UC-03|UC-04|UC-05|UC-06|UC-07|UC-08|UC-09| UC-10|     
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
|RF-001|X| | | | | | | | | |
|RF-002| |X| |X| | | | | | |

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Classes

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Sequências

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Atividades


# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)
