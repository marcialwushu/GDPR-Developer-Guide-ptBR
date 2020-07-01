# Sheet n°7: Minimizar a coleta de dados

#### Você só deve coletar dados pessoais adequados, relevantes e necessários em relação aos propósitos para os quais são processados, conforme definido no momento da coleta.

## Antes da coleta, pense nos diferentes tipos de dados que você precisa coletar e tente limitar sua coleção ao estritamente necessário.

* Pense nos diferentes **tipos de dados** que precisarão ser coletados antes da implementação de um aplicativo e **documente** esse pensamento.

* Se dados específicos não forem necessários para uma determinada categoria de pessoas, não os colete.

* Processe e armazene dados de uma maneira que **reduz a precisão** (semelhante à pseudonimização). Por exemplo, armazene apenas o ano de nascimento, em vez de uma data de nascimento completa, se o aplicativo precisar apenas do ano.

* Se estiver coletando dados particularmente sensíveis, como dados de saúde ou condenações criminais, certifique-se de coletar apenas o **mínimo necessário**. Devido às restrições regulatórias, a solução mais simples ainda é **não coletá-las** se você puder ficar sem elas.

* Minimize a quantidade de dados coletados também nos **dados de log** e não armazene dados sensíveis ou críticos (dados de saúde, senhas, etc.).

* Alguns recursos podem melhorar a experiência do usuário, mas **não são estritamente necessários para que seu aplicativo funcione corretamente** (por exemplo, geolocalização para simplificar uma pesquisa geográfica). Nesse caso, o usuário final deve poder **escolher se deve ou não usar** essa funcionalidade. Se ele usá-lo, os dados que você é levado a coletar para sua operação devem ser mantidos apenas pelo tempo estritamente necessário para sua operação e nunca devem ser usados para outros fins.

* Lembre-se de associar **períodos de retenção** para cada categoria de dados, dependendo da finalidade do processamento e das obrigações legais ou regulamentares relacionadas à sua retenção. Os logs também devem ter um período de retenção. Documente as durações de retenção definidas. Você precisará justificá-los.

## Depois que os dados forem coletados, configure mecanismos de exclusão automática.

* Implemente um sistema automático de **purge** no final do prazo de validade. Você também pode implementar revisões manuais dos dados armazenados periodicamente.

* Para garantir uma eliminação completa, apague **fisicamente** todos os dados que não são mais necessários usando ferramentas especializadas ou destruindo a mídia física.

* Se os dados ainda forem úteis, você poderá reduzir sua sensibilidade usando os métodos **pseudomização** ou mesmo **anonimização**. Em caso de pseudonimização, esses dados permanecem sujeitos às regulamentações de dados pessoais (consulte [Folha 1](#Sheet_n°1_:_Identify_personal_data)).

* Registre os **procedimentos de exclusão automática**. Os logs correspondentes podem ser usados como uma **prova de exclusão** de um item de dados.

