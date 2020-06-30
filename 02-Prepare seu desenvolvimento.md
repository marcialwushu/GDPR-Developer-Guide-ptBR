# Sheet n°2: Prepare seu desenvolvimento

#### Os princípios de proteção de dados pessoais devem ser integrados aos desenvolvimentos de TI a partir da fase de design, a fim de proteger a privacidade das pessoas cujos dados você processará, para proporcionar melhor controle sobre os dados e limitar erros. , perdas, modificações não autorizadas ou uso indevido de seus dados em aplicativos.

## Escolhas metodológicas

* **Coloque a proteção da privacidade no centro de seus desenvolvimentos** adotando um [Privacy By Design](https://edpb.europa.eu/our-work-tools/public-consultations-art-704/2019/guidelines -42019-article-25-data-protection-design_en).

* Se você usar métodos ágeis para seus desenvolvimentos, considere **integrar a segurança no centro do seu processo**. O ANSSI disponibilizou um guia ["segurança digital e agilidade"](https://www.ssi.gouv.fr/uploads/2018/11/guide-securite-numerique-agile-anssi-pa-v1.pdf) (somente em francês), que indica como conduzir seus desenvolvimentos na estrutura de um método ágil, levando em consideração os aspectos de segurança. Não hesite em se inspirar nisso.

* Para qualquer desenvolvimento destinado ao público em geral, **considere as configurações de privacidade** e, em particular, as configurações padrão, como as características e o conteúdo do usuário visíveis por padrão.

* **Realize uma [Avaliação de impacto na privacidade (PIA)](https://www.cnil.fr/en/privacy-impact-assessment-pia)**. Para [certas operações de processamento](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/accountability-and-governance / avaliação de impacto de proteção de dados /) é obrigatório. Noutros casos, é uma boa prática que lhe permitirá identificar e lidar com todos os riscos a montante dos seus desenvolvimentos. A CNIL possui uma seção especial em seu site e fornece um [software livre](https://www.cnil.fr/en/open-source-pia-software-helps-carry-out-data-protection-impact-assment ) dedicado a esse tipo de análise.

## Escolhas tecnológicas

#### Arquitetura e recursos

* **Inclua proteção de privacidade, incluindo requisitos de segurança de dados, no estágio de design do aplicativo ou serviço**. Esses requisitos devem influenciar as [opções de arquitetura](#Sheet_n°5:_Fazer_um_início_da_informática_de_arquitetura) (por exemplo, descentralizada vs. centralizada) ou na funcionalidade (por exemplo, anonimização a curto prazo, minimização de dados). As configurações padrão do aplicativo devem atender aos requisitos mínimos de segurança e cumprir a lei. Por exemplo, a complexidade padrão das senhas deve cumprir pelo menos a [recomendação CNIL sobre senhas](https://www.cnil.fr/fr/node/23803).

* **Mantenha o controle do seu sistema**. É importante manter o controle do seu sistema, tanto para garantir a operação adequada quanto para garantir um alto nível de segurança. Manter um sistema simples permite entender com precisão como ele funciona e identificar seus pontos fracos. Se uma certa complexidade for necessária, é aconselhável começar com um sistema simples, corretamente projetado e seguro. Em seguida, é possível aumentar a complexidade pouco a pouco, enquanto continua protegendo os novos recursos adicionados.

* **Não confie em uma única linha de defesa**. Apesar de todas as etapas adotadas para projetar um sistema seguro, pode acontecer que alguns componentes adicionados posteriormente possam não ser suficientemente seguros. Para minimizar o risco para os usuários finais, é aconselhável defender o sistema em profundidade. Por exemplo, verificar os dados inseridos em um formulário online faz parte das defesas da periferia. Se essa defesa for invadida, a proteção de consultas ao banco de dados poderá assumir o controle.


#### Ferramentas e práticas

* **Use padrões de programação que levem em conta a segurança**. Muitas vezes, já estão disponíveis listas de padrões, práticas recomendadas ou guias de codificação para melhorar a segurança de seus desenvolvimentos. As ferramentas auxiliares também podem ser integradas aos seus ambientes de desenvolvimento integrados ("**IDE**") para verificar automaticamente se seu código está em conformidade com as várias regras que fazem parte desses padrões ou boas práticas. Você pode encontrar facilmente listas de boas práticas para sua linguagem de programação favorita na Internet. Por exemplo [aqui](https://wiki.sei.cmu.edu/confluence/display/seccode/SEI+CERT+Coding+Standards) para C, C ++ ou Java. Para o desenvolvimento de aplicativos da Web, existem guias específicos de boas práticas, como os publicados pela [OWASP](https://www.owasp.org).

* **As opções tecnológicas são críticas.** Alguns parâmetros precisam ser levados em consideração:
     * Dependendo do campo de aplicação ou funcionalidade desenvolvida, uma linguagem ou tecnologia pode ser mais apropriado que outra.
     * Linguagens e tecnologias testadas pelo tempo são mais seguras. Em geral, eles foram auditados para corrigir as vulnerabilidades mais conhecidas. No entanto, você deve ter cuidado ao usar as versões mais recentes de cada um dos componentes básicos da tecnologia que você usará.
     * Você deve evitar codificar sua solução final em uma linguagem que você acabou de aprender e que ainda não domina. Caso contrário, você se expõe a um risco aumentado de falha de segurança devido à falta de experiência.
* **Configure um ambiente de desenvolvimento seguro que permita a versão do código**, seguindo a [dedicada sheet](#Sheet_n°3:_Secure_your_development_environment) neste guia.

