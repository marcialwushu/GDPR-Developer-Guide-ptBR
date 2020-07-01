# Sheet n°15: Leve em consideração a base jurídica da implementação técnica

#### O processamento de dados pessoais deve ser baseado em uma das "bases legais" mencionadas no [artigo 6 do GDPR](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=FR#d1e1888-1-1). A base legal de uma operação de processamento é de certa forma a justificativa da existência da operação de processamento. A escolha de uma base jurídica tem um impacto direto nas condições de implementação da operação de processamento e [nos direitos dos indivíduos](#Sheet_n°13_:_Preparing_the_exercise_of_persons_rights). Assim, antecipar a base jurídica das operações de processamento antes de qualquer desenvolvimento ajudará você a integrar as funções necessárias para garantir que essas operações de processamento cumpram a lei e respeitem os direitos dos indivíduos.

## Definição das bases jurídicas no RGPD

* No contexto de um desenvolvimento para uma organização privada (empresas, associações, etc.), as bases jurídicas frequentemente usadas são:
    * **O contrato**: o processamento é necessário para a execução ou preparação de um contrato entre o titular dos dados e o organismo que realiza a operação de processamento;
    * **O interesse legítimo**: a organização tem um interesse "legítimo" em realizar o processamento e não é provável que afete negativamente os direitos e liberdades dos titulares dos dados;
    * **Consentimento**: o titular dos dados deu seu consentimento explícito para o processamento.

* Se você é uma autoridade pública ou um órgão que realiza tarefas de interesse público, outras bases legais também podem ser usadas:
    * **A obrigação legal**: o processamento é imposto por textos regulatórios.
    * **A missão de interesse público**: o processamento é necessário para a execução de uma tarefa realizada no interesse público.

* Finalmente, em casos muito específicos, **a proteção de interesses vitais** pode ser usada como base legal, por exemplo, quando o processamento é necessário para monitorar a propagação de epidemias ou em casos de emergência humanitária.

## Escolha a base jurídica apropriada

* Antes de tudo, verifique no site da CNIL que **um texto não impõe restrições específicas** (por exemplo: [cookies e outros rastreadores](https://www.cnil.fr/sites/default/files/atoms/files/draft_recommendation_cookies_and_other_trackers_en.pdf)).

* **Apenas uma base jurídica deve ser escolhida** para um determinado objetivo. A base jurídica não pode ser acumulada para a mesma finalidade. A mesma operação de processamento de dados pode buscar vários propósitos e uma base legal deve ser definida para cada um deles.

* Como mencionado acima, se você é uma **autoridade pública**, a obrigação legal e a missão de interesse público serão as mais relevantes na maioria dos casos.

* Se sua operação de processamento faz parte de um relacionamento contratual e seu objetivo é objetiva e estritamente necessário para a prestação do serviço do usuário (por exemplo, nome, nome e endereço para criar uma conta em um site de comércio eletrônico), então **o contrato deve seja apropriado**.

* Se o seu processamento não fizer parte de uma relação contratual com o usuário, **a base jurídica do consentimento ou interesse legítimo** poderá ser invocada. Se o seu processamento for potencialmente invasivo (criação de perfil, coleta de dados de geolocalização, etc.), o consentimento provavelmente será a base legal apropriada.

* Se o seu processamento contiver **dados confidenciais** (dados de saúde, dados relativos à vida ou orientação sexual, etc.), será necessário identificar, além da base legal, uma exceção prevista no [Artigo 9 da RGPD](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32016R0679&from=FR#d1e2051-1-1).

Exercícios e modalidades de informações a serem fornecidas de acordo com a base legal

* A tabela a seguir resume os exercícios de direitos a serem concedidos de acordo com a base legal:

| | Direito de acesso | Direito à retificação | Direito de apagar | Direito à restrição de processamento | Direito à portabilidade de dados | Direito de objetar |
|:---------------------:|:-------------:|:----------------------:|:--------------------:|:-----------------------------------:|:----------------------:|:---------------------------:|
| **Consentimento**      | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | **Retirada do consentimento**|
| **Contrato**           | ✔             | ✔                      | ✔                    | ✔                                   | ✔                      | ✘                           |
| **Interesse legítimo**  | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✔                           |
| **Obrigação legal** | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✘                           |
| **Interesse público**    | ✔             | ✔                      | ✘                    | ✔                                   | ✘                      | ✔                           |
| **Proteger interesses vitais**   | ✔             | ✔                      | ✔                    | ✔                                   | ✘                      | ✘                           |

* A base jurídica utilizada deve sempre aparecer nas informações transmitidas à pessoa.

* **Onde seu processamento é baseado em interesses legítimos**, você também deve indicar os interesses legítimos perseguidos (luta contra fraude, segurança do sistema etc.).

* Recomenda-se **documentar sua escolha da base jurídica**. Como exemplo, essas opções podem ser indicadas em um mapa de processamento ou associadas à sua documentação técnica.

## O caso específico de cookies e outros rastreadores

* A Diretiva Européia de Privacidade Eletrônica exige o consentimento do usuário antes que qualquer ação seja tomada para armazenar informações - por meio de cookies, identificadores ou outros rastreadores (impressões digitais de software, pixels) ou para acessar informações armazenadas no equipamento terminal do usuário.

* No entanto, uma exceção é feita quando os cookies têm o único objetivo de realizar comunicação eletrônica ou são estritamente necessários para fornecer um serviço solicitado pelo usuário.

* Além disso, o uso de um único rastreador para múltiplos propósitos não isenta de obter consentimento para os fins que o exigem. Por exemplo, se um cookie de autenticação também for usado para fins de segmentação de publicidade, o consentimento deverá ser obtido para o último objetivo, da mesma maneira que para um site não registrado.



