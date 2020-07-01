# Sheet n°5: Faça uma escolha informada da arquitetura

#### Ao projetar a arquitetura do seu aplicativo, você deve identificar os dados pessoais que serão coletados e definir um caminho e um ciclo de vida para cada um deles. A escolha dos ativos de suporte (armazenamento local, servidor, serviço em nuvem) é uma etapa crucial, que deve ser adaptada às suas necessidades, mas também ao seu conhecimento técnico. O registro e a realização de uma avaliação de impacto na privacidade podem ajudá-lo nessa escolha.

## Examinando o ciclo de vida de dados e processos, da coleta à eliminação

* Represente e descreva como o produto geralmente funciona antes de iniciar seu projeto, com um diagrama de fluxos de dados e uma descrição detalhada dos processos realizados.

* Quando os dados são apenas ** armazenados no terminal do usuário ** (armazenamento local) ou permanecem ** confinados nas redes de comunicação sob o controle do usuário ** (por exemplo, Wi-Fi ou outra rede local), o principal ponto de atenção é segurança de dados. A duração pela qual os dados são armazenados e a exclusão real deve ser determinada pelos indivíduos.

* **Quando os dados passam por serviços online**, a opção de hospedar os dados você mesmo ou usar um provedor de serviços deve ser feita de acordo com o seu conhecimento de segurança e a qualidade esperada do serviço. Ofertas de nuvem reconhecidas podem oferecer níveis mais altos de segurança. No entanto, eles geram novos riscos que precisam ser dominados. [Recomendações para empresas que planejam usar serviços de computação em nuvem](https://www.cnil.fr/sites/default/files/typo/document/Recommendations_for_companies_planning_to_use_Cloud_computing_services.pdf) podem orientar nesta etapa de seleção.

## No caso de uso de hospedagem externa

* **Escolha um provedor de serviços que garanta medidas adequadas de segurança e confidencialidade e seja suficientemente transparente**.

* **Verifique a localização geográfica dos servidores que hospedarão seus dados**. Pode ser necessário transferir dados para fora da União Europeia (UE) e do Espaço Econômico Europeu (EEE). Embora os dados possam circular livremente na UE/EEE, são possíveis transferências para fora da UE/EEE, desde que seja garantido um nível suficiente e adequado de proteção de dados. O CNIL fornece um mapa no local mostrando os [diferentes níveis de proteção de dados em países do mundo](https://www.cnil.fr/en/data-protection-around-the-world).

* **Se você precisar hospedar dados de saúde**, verifique se o provedor usado é [certificado](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-certifies) ou [aprovado ](https://esante.gouv.fr/labels-certifications/hds/liste-des-herbergeurs-agrees) para esta atividade.

* Outros pontos a serem considerados incluem:
     - a existência de uma política de segurança acessível;
     - segurança física e medidas de segurança no site de hospedagem;
     - criptografia de dados e outros processos para garantir que o provedor não tenha acesso aos dados que lhe são confiados;
     - gerenciamento de atualizações, gerenciamento de autorizações, autenticação de pessoal e segurança do desenvolvimento de aplicativos;
     - a fácil reversibilidade/portabilidade dos dados em um formato estruturado e comumente usado, mediante solicitação e a qualquer momento.


