<p align="center"><img src="https://github.com/LINCnil/GDPR-Developer-Guide/raw/master/templates/BANNIERE-EN.JPG" width="100%" align="middle"></p>


# GDPR Developer Guide ptBR

#### Para ajudar os desenvolvedores da Web e de aplicativos a tornar seu trabalho compatível com o GDPR, a CNIL elaborou um novo guia de boas práticas sob uma licença de código aberto, que deve ser enriquecida por profissionais.

Este guia é publicado sob [licença GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) e sob a [open license 2.0](https://www.etalab.gouv.fr/wp-content/uploads/2017/04/ETALAB-Licence-Ouverte-v2.0.pdf) (explicitamente compatível com [CC-BY 4.0 FR](https://creativecommons.org/licenses/by/4.0/deed.fr)). Você pode contribuir livremente para sua redação..

A [versão Francesa](https://github.com/LINCnil/Guide-RGPD-du-developpeur) é a versão autêntica deste guia.

#### Este guia é apenas para desenvolvedores?

Este guia é voltado principalmente para desenvolvedores que trabalham sozinhos ou em equipes, líderes de equipe, provedores de serviços, mas também para qualquer pessoa interessada no desenvolvimento de aplicativos ou web.

Ele fornece conselhos e melhores práticas e, portanto, fornece chaves úteis para entender o GDPR para cada parte interessada, independentemente do tamanho de sua estrutura. Também pode estimular discussões e práticas nas organizações e nos relacionamentos com os clientes.

#### O que contém o guia?

Este guia está dividido em **16 folhas temáticas**, que cobrem a maioria das necessidades dos desenvolvedores em cada estágio do projeto, desde a preparação do desenvolvimento até o uso de analytics.

O Regulamento Geral de Proteção de Dados (ou RGPD) especifica que a proteção dos direitos e liberdades das pessoas singulares exige que **"sejam tomadas as medidas técnicas e organizacionais adequadas para garantir o cumprimento dos requisitos do presente regulamento"** (considerando 78) .

A determinação dessas medidas está necessariamente **relacionada ao contexto das operações de processamento implementadas**, e o responsável pelo tratamento (a entidade pública ou privada que processa dados pessoais) deve, portanto, garantir a segurança dos dados que é chamado a processar .

As boas práticas deste guia **,portanto, não se destinam a cobrir todos os requisitos dos regulamentos nem a serem prescritivas**, elas fornecem um primeiro nível de medidas para levar em conta os problemas de proteção da privacidade nos desenvolvimentos de TI que se destinam a serem aplicados a todos os projetos de processamento de dados. Dependendo da natureza do processamento realizado em certos casos, medidas adicionais deverão ser implementadas para cumprir totalmente os regulamentos.

## Índice

0. [Desenvolva em conformidade com o GDPR](#Sheet_n°0_:_Desenvolva_em_conformidade_com_o_GDPR)

1. [Identificar dados pessoais](#Sheet_n°1_:_Identify_personal_data)

2. [Prepare seu desenvolvimento](#Sheet_n°2_:_Prepare_your_development)

3. [Protegendo seu ambiente de desenvolvimento](#Sheet_n°3_:_Protegendo_seu_ambiente_de_desenvolvimento)

4. [Gerenciar seu código fonte](#Sheet_n°4_:_Manage_your_source_code)

5. [Faça uma escolha informada da arquitetura](#Sheet_n°5_:_Make_an_informed_choice_of_architecture)

6. [Protegendo seus sites, aplicativos e servidores](#Sheet_n°6_:_Protegendo_seus_sites,_applications_and_servers)

7. [Minimizar a coleta de dados](#Sheet_n°7_:_Minimize_data_collection)

8. [Gerenciar perfis de usuário](#Sheet_n°8_:_Manage_users_profiles)

9. [Controle suas bibliotecas e SDKs](#Sheet_n°09_:_Control_your_libraries_and_SDKs)

10. [Garanta a qualidade do código e sua documentação](#Planilha_n°10_:_Garanta_qualidade_do_documento_e_documentação)

11. [Teste seus aplicativos](#Sheet_n°11_:_Test_your_applications)

12. [Informar usuários](#Sheet_n°12_:_Inform_users)

13. [Prepare-se para exercer os direitos das pessoas](#Sheet_n°13_:_Prepare_for_the_exercise_of_people_rights)

14. [Definir um período de retenção de dados](#Sheet_n°14_:_Define_a_data_retention_period)

15. [Leve em consideração a base jurídica da implementação técnica](#Sheet_n°15_:_Take_into_account_the_legal_bases_in_the_technical_implementation)

16. [Use analytics em seus sites e aplicativos](#Sheet_n°16:_Use_analytics_on_your_websites_and_applications)



## Como posso contribuir para este guia?

**Este guia está disponível em duas versões**:

* Uma [versão da web no site da CNIL](http://www.cnil.fr/en/rgpd-developers-guide) e no guia  [the "Releases" tab](https://github.com/LINCnil/GDPR-Developer-Guide/releases) deste repositório;
* Esta [versão do GitHub](https://github.com/marcialwushu/GDPR-Developer-Guide-ptBR), que oferece a possibilidade de todos contribuírem

**A contribuição é feita em algumas etapas**:

* Registre-se no Github;
* Vá para a página do projeto;
* Você pode:
    * Use uma "Issue" para abrir comentários ou participar da discussão
    * Use a opção "Fork" para fazer suas próprias modificações e propor sua inclusão através do botão "Pull Requests".
    
**Sua proposta de contribuição será examinada pelo autor deste projeto antes da publicação**. A versão web do guia do desenvolvedor do RGPD será atualizada regularmente.

## Uso

Para liberar esse repositório, você pode usar a ferramenta **Pandoc**. Essa ferramenta permitirá converter os registros em um arquivo docx ou documento HTML.

Você pode encontrar as instruções para instalar esta ferramenta  [aqui]( https://pandoc.org/installing.html)

* **To generate a .docx file**:

```bash
pandoc -s --toc --toc-depth=1 -o Guide_RGPD_developper.docx [0-9][0-9]*.md
```

* **To generate an .html file**:

```bash
pandoc -s --template="templates/mytemplate.html" -H templates/pandoc.css -o index.html README.md [0-9][0-9]*.md
```


