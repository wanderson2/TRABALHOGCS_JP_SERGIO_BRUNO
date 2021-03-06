Certidão Concurso Público
=================
Plano de Gerenciamento de Configuração
======================================
Versão 1.03
------------------

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_02/12/2013_|_1.00_|_Criação do documento_|_João Paulo_|
|_03/12/2013_|_1.01_|_Atualizar documento_|_João Paulo_|
|_03/12/2013_|_1.02_|_Atualizar documento_|_João Paulo_|
|_05/12/2013_|_1.03_|_Atualizar documento_|_Bruno Queiroz_|
|_07/12/2013_|_1.04_|_Atualizar documento_|_Bruno Queiroz_|



1. Introdução
==============

O Plano de Gerenciamento de Configuração explica todas as atividades do Gerenciamento de Controle de Configuração e Mudança que serão realizadas durante o ciclo de vida do produto. Suas atividades envolvem reconhecer a configuração do software, manter sua integridade durante o projeto e controlar sistematicamente as mudanças.

1.1 Finalidade
---------------
A finalidade deste documento é criar um padrão a ser seguido por todos os membros da equipe com o propósito de garantir o maior controle do produto no decorrer do projeto. Para realizar serão detalhados os recursos necessários (equipes, ferramentas e computadores), as responsabilidades e o cronograma de atividades.


1.2 Escopo
----------
Este Plano de Gerenciamento de Configuração é destinado para todos os integrantes da equipe responsável pelo desenvolvimento do sistema para promover maior eficiência nas atividades de emissão de certidão da 5ª Região da Justiça Federal, através do cadastro das informações, automatização e controle das certidões, além de considerável economia financeira decorrente de redução do gasto com impressões em papel, gasto com materiais de expediente para manter e controlar as certidões e o gasto de mão-de-obra dos funcionários do cadastro da Justiça Federal.

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
SCRUM - É um processo ágil que permite manter o foco na entrega do maior valor de negócio, no menor tempo possível.
GC - Gerência de Configuração.
CCM - Comitê para o Controle de Mudanças.
Baseline - Conjunto de artefatos que recebe uma aprovação de estabilidade. Um baseline é usado como uma base no desenvolvimento das próximas fases dos artefatos e tem suas modificações controladas por um processo.
CM - Controle de Mudanças.

1.4 Referências
---------------
Template de Gerenciamento de Configuração.

1.5 Visão Geral
---------------
Na seção de 2 (Gerenciamento de configuração de software): São relacionados os papéis, as responsabilidades das atividades e as ferramentas dentro da GC da Fábrica.
Na seção 3 (O Programa de Gerenciamento de Configuração): É apresentado como serão criadas e controladas as Baselines.
Na seção 4  (Padrões e Procedimentos): Descreve os padrões e procedimentos que devem ser seguidos no projeto.
Na seção 5 (Treinamento e Recursos): Descreve as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas.
Na seção 6 ( Auditorias de Configuração): Descreve o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.


2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------
Papéis                                                             
Gerente de configuração
Equipe
João Paulo
Responsabilidade
Estabelecer Políticas de GC
Escrever Plano de GC
Configurar Ambiente de GC
Criar Baselines

Papéis                                                             
CCM
Equipe
João Paulo
Sergio Rodrigues
Bruno Duarte
Responsabilidade
Estabelecer Processo de Controle de Mudanças
Revisar Solicitação de Mudança

Papéis                                                             
Desenvolvedor
Equipe
João Paulo
Bruno Duarte
Sergio Rodrigues
Responsabilidade
Seguir os padrões e procedimentos definidos no Plano de Gerência de Configuração

2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------

Ferramenta:
Subversion - Sistema de controle de versão
TortoiseSVN - Acesso ao repositório, é o Client para o Subversion integrado ao Windows.
 
Ambiente: 
Sistema operacional - Windows 7
Pacote Office 2010
Antvírus: Avast
Controle de versão: Subversion 1.8.5
Plataforma de desenvolvimento JAVA: Eclipse
Banco de dados: PostgreSQL
Comunicação: Gmail

A estrutura do ambiente será da seguinte forma:

Desenvolvimento: É o ambiente que servirá para o desenvolvimento do Sistema.	O componente atingirá a maturidade quando os requisitos forem supridos e testados pelos desenvolvedores através dos testes unitários.
Configuração: Processador 2.8 GHz, Memória RAM 4GB, HD de 500 GB
Integração: É o ambiente que servirá para os testes de integração.
Quando a comunicação entre os módulos atinge o um estagio satisfatório de funcionamento.
Configuração: Processador 2.8 GHz, Memória RAM 4GB, HD de 500 GB
Banco de Dados: É o ambiente onde conterá o Banco de dados.
Configuração: Processador 2.8 GHz, Memória RAM 4GB, HD de 500 GB

3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------

### 3.1.1 Métodos de Identificação

#### 3.1.1.1 Nomenclatura dos artefatos

Todos os documentos disponibilizados no repositório (exceto o código do sistema, pois este segue um padrão de desenvolvimento) devem ser identificados baseados na seguinte nomenclatura:
 
&lt;ID_ARTEFATO&gt; - &lt;NOME_ARTEFATO&gt;

Onde:

* &lt;ID_ARTEFATO&gt; é a sigla de identificação do artefato conforme Tabela 2.
* &lt;NOME_ARTEFATO&gt; é nome de identificação do artefato conforme Tabela 2.

| Id do artefato | Nome do artefato	 |
|----------------|-------------------|
|APD   |   Ativação de Projeto de Desenvolvimento
|EOR   |   Especificação de Objetivos e Requisitos
|LPS   |   Levantamento Preliminar do Software
|PCP   |   Plano de Comunicação do Projeto
|PDS   |    Plano de Desenvolvimento de Software
|PGC   |   Plano de Gerência de Configuração
|PGQ   |  Plano de Gerência da Qualidade
|PGR   |   Plano de Gerência de Riscos
|RAC   |  Relatório de Avaliação do Cliente
|RAP   |   Relatório de Acompanhamento do Projeto
|PFM   |  Pedido Formal de Modificação
|SAI   |  Solicitação de Análise de Impacto
|RTF   |  Relatório de RTF (Revisão Técnica Formal)
|DAS   |   Documento de Análise de Software
|DPS   |   Documento de Projeto de Software
Tabela 2 - Ids e nomes de documentos

#### 3.1.1.2 Versão dos artefatos

Todos os artefatos (exceto os arquivos de código fonte do programa) deverão ter uma nomenclatura de versionamento segundo o seguinte padrão:

X.YY

Onde:
* X é um número que representa uma versão final do Artefato;
* YY é um número que representa uma versão intermediária posterior a uma versão X do artefato.

O versionamento dos artefatos dar-se-á da seguinte forma:
* a cada versão interdiária o valor de YY aumenta em uma unidade;
* a cada versão estável do artefato o valor de YY é zerado e o valor de X é incrementado em uma unidade.

#### 3.1.1.3 Nomenclatura de branches e tags

* Os branches locais não são controlados pelo nosso GCS, portanto podem ser nomeados de qualquer forma.
Os branches remotos serão nomeados seguindo o seguinte padrão:
nomeDoTrackBranch_idDaFuncionalidadeNoJira_descricaoDaFuncionalidade, onde "nomeDoTrackBranch" é o nome do branch de origem.
* As tags deverão ser geradas a cada nova versão entregue do sistema. Estas serão nomeadas seguindo o seguinte padrão: V1.0, onde o "V" é um prefixo e o "1.0" é a versão do software gerado.

#### 3.1.1.4 Outras nomenclaturas

Os artefatos não citados nesta seção terão sua identificação padronizada e diferenciada apenas pelo diretório em que se encontram e não pelo nome do arquivo.

### 3.1.2 Itens de Configuração

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|_Plano de projeto, planos auxiliares, EAP e Cronograma (documentação do projeto)_|_João Paulo_|_O mais cedo possível_|
|_Requisitos, Especificações, Modelos (documentação de Software)_|_Sérgio_|_Na fase de análise de requisitos_|
|_Massa de dados de teste_|_Bruno_|_Após a fase de construção_|
|_Código fonte_|_Bruno_|_durante a fase de construçao_|

### 3.1.3 Baselines do Projeto

| Fases                 | Itens de configuração da baseline	     |
|----------------------------------------|-----------------------|
|_Iniciação_|_Plano de projeto e planos auxiliares, incluindo Plano de Gerenciamento de Configuração_|
|_Elaboração_|_Requisitos, Especificações_|
|_Projeto de Software_|_Modelos, Código fonte (provas de conceito das partes mais complicadas, arquitetura inicial)_|
|_Construção - 1ª Entrega_|_Código fonte_|
|_Construção - 2ª Entrega_|_Código fonte_|
|_Construção - 3ª Entrega_|_Código fonte_|
|_Transição_|_Executável, documentação do sistema_|

### 3.1.4 Estrutura do Repositório de Versões

<table
 <tr>
  <th>Diretório</th>
  <th>Subdiretório</th>
  <th>Artefatos</th>
 </tr>
 <tr>
  <td rowspan="3">Documentos</td>
  <td>Gerência de Configuração</td>
  <td>Modelo do Plano de Gerenciamento de configuração
      Notas de Releases
      Arquivos de aprovação dos documentos
  </td>
 </tr>
 <tr>
  <td>Gerência de Projetos </td>
  <td>Documento de Visão
      Termo de Abertura
      Plano de Projeto
      Cronograma
      Relatório de Status
      Atas de Reuniões
      Arquivos de aprovação dos documentos
  </td>
 </tr>
 <tr>
  <td>Analise e Projeto</td>
  <td>  Manual de Implantação
        Documento de Arquitetura
        Modelo de Banco de Dados
        Modelo de Análise e Projetos
        Arquivos de aprovação dos documentos
  </td>
 </tr>
 <tr>
  <td>Site</td>
  <td>Fontes</td>
   <td></td>
 </tr>
</table>

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

As solicitações de mudança (SM) serão realizadas exclusivamente através da ferramenta de controle de mudanças Jira. Os possíveis estados de uma (SM) estão listados abaixo:

| Estado                 | Descrição	     |
|------------------------|-----------------------|
|_Aberto_|_Este estado indica que uma SM foi cadastrada no Jira mas ainda não começaram a resolvê-la_|
|_Iniciado_|_Indica que começou-se a resolução da SM_|
|_Resolvido_|_Indica que a SM foi resolvida e está pronta para testes_|
|_Em Teste_|_Indica que a SM está em testes pela equipe de testadores. (Este estado não faz parte dos estados padrão do Jira mas é útil para indicar que uma SM está em testes e evitar que testadores peguem a mesma SM para testar)_|
|_Reaberto_|_Indica que foi encontrado algum erro no teste e a SM ficará aberta novamente para que se resolvam os erros_|
|_Fechado_|_Indica que finalizou o ciclo da SM. Este estado inclui um motivo da finalização do ciclo, que são: "Resolvido" e "Não pôde reproduzir"_|



O diagrama abaixo apresenta a máquina de estados (estados e transições possíveis) de uma SM neste projeto:

![Image](http://dec.imghost.us/pJ75.png?raw=true)


### 3.2.2 Comitê de Controle de Mudança (CCB)
As Solicitações de Mudança deverão passar pelo CCB, que analisará o impacto dessa mudança, verificando: 
 * os riscos envolvidos, como quantidade de código alterado e funcionalidades complexas que serão alteradas;
 * analisará o custo benefício da mudança, fazendo um balanceamento entre sua prioridade + necessidade e o custo + risco de sua implantação.
As solicitações serão analisadas pelo comitê (CCB), que deve ter todos os seus membros presentes para garantir que a SM foi analisada sob todos os pontos de vista possíveis e necessários. O CCB será formado por equipe multidisciplinar, contendo no mínimo uma pessoa das seguintes áreas (programador, analista, gerente de projetos). O quadro abaixo apresenta os menbros do CCB.

| Menbro                 | Responsabilidade	     |
|------------------------|-----------------------|
|_João Paulo (Gerente)_|_Organizar, facilitar e conduzir a reunião do CCB e anotar o parecer final para que seja este levado adiante_|
|_Sergio (Analista)_|_Verificar a real necessidade da SM e se esta faz sentido, verificando sua conformiade com padrões adotados no sistema e seu escopo_|
|_Bruno (Programador)_|_Verificar o risco da implementação da mudança, levando em conta as alterações que deverão ser realizadas no código; verificar a viabilidade da mudança e estimar o tempo necessário_|

4. Padrões e Procedimentos
==========================

Nesta seção, serão apresentados os padrões utilizados no projeto tais como, identificadores, nomes de arquivos, nomes de tags, nomes de branches, versionamento (sistema, documentos, e baselines).

Projeto .:        certidaoConcursosPublicos

Identificador.: PRJ SADES 013 

Caminho.:      
http://srvapp.jfce.jus.br/desenvolvimento/documentacaosades/projetos/PRJ SADES 013 - certidaoConcursosPublicos

Identificadores de Tipos de Artefatos
Identificador  - Descrição
ARQ  - Documento de Arquitetura do Sistema

DOC  - Documento não classificado

I18N  - Tabela de Internacionalização

MAD  - Modelo de Análise e Projeto

MAN  - Manual

MBD  - Esquema do Banco de Dados

MRT  - Matriz de Ratreabilidade de Requisitos

REQ  - Especificação de Requisitos de Software

TSTD - Projeto de Testes


5. Treinamento e Recursos
=========================
Descrição dos treinamentos efetuados para os integrantes do Grupo.

Treinamento no Repositório.: 	Treinamento ensina como acessar o repositório através de uma máquina cliente, como dar os comandos principais do repositório,  como incluir novos itens dentro do repositório e também como remover do mesmo, tendo como alvo toda a equipe.



6. Auditorias de Configuração
=============================
Finalidade

 - Determinar que uma baseline contém todos os artefatos necessários

 - Determinar que uma baseline atende aos requisitos

Passos:

1) Executar Auditoria de Configuração Física.

Uma Auditoria de Configuração Física (PCA) identifica os componentes de um produto que serão implantados do Repositório do Projeto.  Os passos são:

 - Identificar a baseline a ser implantada (geralmente é apenas um nome e/ou número, mas também pode ser uma lista completa de todos os componentes e suas respectivas versões).

 - Confirmar que todos os artefatos necessários, conforme especificado pelo Caso de Desenvolvimento, estão presentes na baseline.  Liste os artefatos ausentes em Descobertas da Auditoria de Configuração.

2) Executar Auditoria de Configuração Funcional

Uma Auditoria de Configuração Funcional (FCA) confirma que uma baseline atende aos requisitos estabelecidos para ela.  Os passos para a execução dessa auditoria são:

 - Preparar um relatório que liste cada requisito estabelecido para a baseline, seu procedimento de teste correspondente e o resultado de teste (aprovado/reprovado) da baseline.  

 - Confirmar que cada requisito passou por um ou mais testes e que o resultado de todos esses testes foi 'aprovado'.  Em Descobertas da Auditoria de Configuração, liste quaisquer requisitos que não tenham passado por procedimentos de teste e os requisitos que estão com teste incompleto ou que foram reprovados. 

 - Gerar uma lista das CRs estabelecidas para essa baseline.  Confirme que cada CR foi fechada.  Em Descobertas da Auditoria de Configuração, liste quaisquer CRs que não estão fechadas.

3) Reportar Descobertas

Se houver alguma discrepância, ela será capturada em Descobertas da Auditoria de Configuração conforme descrito anteriormente.  Além disso, os seguintes passos deverão ser executados:

 - Identificar ações corretivas.  Talvez, isso requeira a entrevista de vários membros da equipe do projeto para que a origem da discrepância e as ações apropriadas sejam identificadas.  

 - Para artefatos ausentes, a ação apropriada é geralmente controlar a configuração do artefato ou criar uma CR ou tarefa que produzirá o artefato ausente.

 - No caso de requisitos não testados ou reprovados no teste, o requisito pode ser estabelecido para uma baseline posterior ou negociado para ser removido do conjunto de requisitos.

 - Para CRs em aberto, a CR pode ser simplesmente fechada, testada ou adiada para uma baseline posterior.

 - Para cada ação corretiva, atribua uma responsabilidade e determine uma data de conclusão.
