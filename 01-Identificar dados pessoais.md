# Sheet n°1: Identificar dados pessoais

#### Compreender as noções de "dados pessoais", "finalidade" e "processamento" é essencial para garantir que o software cumpra a lei ao processar dados do usuário. Em particular, tome cuidado para não confundir "anonimização" e "pseudonimização", que têm definições muito precisas e diferentes no RGPD.

## Definição
* A noção de **dados pessoais** é definida no [Regulamento Geral de Proteção de Dados](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32016R0679) (GDPR ) como "[qualquer informação relativa a uma pessoa singular identificada ou identificável (referida como" titular dos dados ")](https://www.cnil.fr/en/personal-data-definition)". Abrange um amplo escopo que inclui dados de identificação direta (por exemplo, nome e sobrenome) e dados de identificação indireta (por exemplo, número de telefone, placa do veículo, identificador de terminal etc.).

* Qualquer operação neste tipo de dados (coleta, gravação, transmissão, modificação, disseminação etc.) constitui **processamento na acepção do GDPR** e, portanto, deve atender aos requisitos estabelecidos por esse regulamento. Tais operações de processamento devem ser legais e ter um objetivo especificado. Os dados pessoais coletados e processados devem ser relevantes e limitados ao estritamente necessário para alcançar o objetivo.

## Exemplos de dados pessoais

* No que se refere a pessoas singulares, **os seguintes dados são dados pessoais**:
     * Sobrenome, nome, pseudônimo, data de nascimento;
     * fotos, gravações sonoras de vozes;
     * número de telefone fixo ou móvel, endereço postal, endereço de e-mail;
     * Endereço IP, identificador de conexão do computador ou identificador de cookie;
     * Impressão digital, palma ou rede venosa da mão, impressão da retina;
     * Número da placa, número do seguro social, número de identificação;
     * Dados de uso do aplicativo, comentários, etc ...

* **A identificação de pessoas singulares pode ser realizada**:
     * a partir de um único dado (exemplos: sobrenome e nome);
     * a partir do cruzamento de um conjunto de dados (exemplo: uma mulher que vive em tal e qual endereço, nascida em tal e tal dia e membro de tal e tal associação).

* Alguns dados são considerados **particularmente sensíveis**. O GDPR proíbe a coleta ou o uso de tais dados, a menos que, em particular, todos os titulares de dados envolvidos tenham dado seu consentimento expresso (consentimento ativo, explícito e de preferência por escrito, que deve ser gratuito, específico e informado).

* Esses requisitos dizem respeito aos seguintes dados:

     * dados relativos à **saúde dos indivíduos**;
     * dados sobre **vida sexual** ou **orientação sexual**;
     * dados revelando uma suposta origem racial ou étnica;
     * opiniões políticas, crenças religiosas, crenças filosóficas ou filiação sindical;
     * **dados genéticos** e **biométricos utilizados com a finalidade de identificar exclusivamente um indivíduo**.
     
## Anonimização de dados pessoais

* Um **processo de anonimização de dados pessoais** visa impossibilitar a identificação de indivíduos nos conjuntos de dados. É, portanto, um processo irreversível. Quando essa anonimização é efetiva, os dados não são mais considerados dados pessoais e os requisitos do GDPR não são mais aplicáveis.

* Por padrão, recomendamos que você nunca **considere conjuntos de dados brutos como anônimos**. A anonimização resulta do processamento de dados pessoais para impedir irreversivelmente a identificação, seja por:

     * _singling out_: não é possível isolar alguns ou todos os registros que identificam um indivíduo no conjunto de dados;
     * _linkability_: o conjunto de dados não permite vincular dois ou mais registros referentes ao mesmo assunto ou a um grupo de dados;
     * _inference_: não é possível inferir, com probabilidade significativa, o valor de um atributo a partir dos valores de um conjunto de outros atributos.
     
* Essas operações de processamento de dados implicam na maioria dos casos **perda de qualidade no conjunto de dados produzido**. O grupo de trabalho do artigo 29.º (artigo 29.º do WP) [parecer sobre técnicas de anonimização](https://ec.europa.eu/justice/article-29/documentation/opinion-recommendation/files/2014/wp216_en.pdf) descreve o principais técnicas de anonimização usadas atualmente, bem como exemplos de conjuntos de dados considerados erroneamente anônimos. É importante observar que as técnicas de anonimização têm deficiências. A escolha entre anonimizar ou não os dados e a escolha de uma técnica de anonimização deve ser feita caso a caso, de acordo com os diferentes contextos de uso (natureza dos dados, utilidade dos dados, riscos para as pessoas etc.).     


## Pseudonimização de dados pessoais

* **A pseudonimização é um compromisso entre reter dados brutos e produzir conjuntos de dados anonimizados**.

* Refere-se ao processamento de dados pessoais de forma que **os dados relativos a uma pessoa natural não possam mais ser atribuídos sem informações adicionais**. O GDPR insiste que essas informações adicionais devem ser mantidas separadamente e estar sujeitas a medidas técnicas e organizacionais para evitar a re-identificação dos titulares dos dados. Diferentemente da anonimização, a pseudonimização pode ser um processo reversível.

* Na prática, um processo de pseudonimização consiste em **substituir diretamente os dados de identificação (sobrenome, nome próprio etc.) em um conjunto de dados por dados de identificação indireta** (alias, número em um sistema de arquivamento etc.) para reduzir sua sensibilidade. Eles podem resultar de um hash criptográfico dos dados de indivíduos, como endereço IP, ID do usuário e endereço de email.

* Os dados resultantes da pseudonimização são considerados **dados pessoais e, portanto, permanecem sujeitos às obrigações do DPMR**. No entanto, o Regulamento Europeu incentiva o uso de pseudonimização no processamento de dados pessoais. Além disso, o RGPD considera que a pseudonimização permite reduzir os riscos para os titulares de dados e contribuir para o cumprimento do regulamento.
