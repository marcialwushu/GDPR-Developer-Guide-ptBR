# Sheet n°13: Prepare-se para exercer os direitos das pessoas

#### As pessoas cujos dados você processa têm direitos sobre os dados dele: direito de acesso, retificação, objeção, exclusão, portabilidade de dados e restrição de processamento. Você deve fornecer a eles os meios para exercer efetivamente seus direitos e fornecer em seus sistemas de computador as ferramentas técnicas que permitirão que seus direitos sejam levados em consideração adequadamente.

#### A preparação antecipada de como eles entrarão em contato com você e como você lidará com as solicitações deles permitirá que você gerencie o exercício desses direitos com eficiência.

## Medidas mínimas a serem implementadas

* Todas as organizações que usam dados pessoais têm **a obrigação de indicar onde e como** indivíduos podem exercer seus direitos em relação a esses dados. Por exemplo, você pode mencionar um endereço de email ou um formulário da Web ao informar indivíduos, bem como em sua política de privacidade.

* Para facilitar o exercício dos direitos das pessoas, esses direitos também podem ser **implementados**, no todo ou em parte, diretamente no **aplicativo ou software que você desenvolve**. Essa implementação específica não é obrigatória, mas permite atender às expectativas dos usuários e reduzir o tempo e a complexidade do processamento desse tipo de solicitação.

* Acima de tudo, no caso de acesso ou operações realizadas diretamente por uma pessoa que exerce seus direitos, não se esqueça de gerenciar sua **autenticação** de maneira segura. No geral, **rastreia** também todas as operações que afetam seus dados pessoais.

## Aqui estão alguns exemplos de direitos e sua possível implementação

* **Direito de acesso**: as pessoas têm o direito de obter uma cópia de todas as informações que você tem sobre elas. Isso permite, entre outras coisas, que uma pessoa saiba se os dados a seu respeito estão sendo processados e obtenha uma cópia legível em um formato compreensível. Em particular, permite verificar a precisão dos dados.
**_ Possível implementação _**: Forneça uma funcionalidade para exibir todos os dados relacionados a uma pessoa. Se houver muitos dados, você poderá dividi-los em vários monitores. Se os dados forem muito grandes, ofereça à pessoa o download de um arquivo que contenha todos os seus dados.

* **Direito de apagar**: as pessoas têm o direito de solicitar a exclusão de todos os dados que você possui.
**_ Possíveis implementações _**:
     1. Forneça uma funcionalidade para apagar todos os dados relacionados a uma pessoa.
     2. Forneça também a notificação automática dos processadores para apagar também os dados relacionados a essa pessoa.
     3. Forneça a exclusão de dados também nos backups ou forneça uma solução alternativa que não restaure os dados apagados relacionados a essa pessoa.

* **Direito de contestar**: os indivíduos têm o direito de contestar, em certos casos, seus dados que são usados para uma finalidade específica.
**_ Possível implementação _**: fornece uma funcionalidade que permite ao sujeito de dados se opor ao processamento. Quando o titular dos dados exercita seu direito de se opor dessa maneira, o responsável pelo tratamento deve excluir os dados já coletados e, posteriormente, não deve coletar mais dados relacionados a essa pessoa.

* **Direito à portabilidade de dados**: os indivíduos têm o direito de recuperar seus dados em um formato legível por máquina para uso próprio ou para transferência para outra organização.
**_ Possível implementação _**: forneça um recurso que permita que o titular dos dados baixe seus dados em um formato legível por máquina padrão (CSV, XML, JSON etc.).

* **Direito de retificação**: Os indivíduos têm o direito de solicitar a modificação de seus dados quando estiverem incorretos, a fim de limitar o uso ou a disseminação de informações erradas.
**_ Possível implementação _**: Permite modificar diretamente os dados na conta do usuário.

* **Direito à restrição de processamento**: os indivíduos têm o direito de solicitar que o processamento de seus dados seja bloqueado por um determinado período de tempo, por exemplo tempo para examinar uma disputa da parte deles sobre o uso de seus dados ou uma solicitação para exercer direitos.
**_ Possível implementação _**: Permite aos administradores colocar dados sobre uma pessoa em "quarentena": esses dados não podem mais ser lidos ou modificados.

## Em conclusão

* O [site Data & Design](https://design.cnil.fr/en) desenvolvido pelo Laboratório de Inovação Digital da CNIL desenvolve esses conceitos e contém [exemplos de interfaces para o exercício de direitos](https://design.cnil.fr/en/concepts/exercising-rights/).

* Finalmente, seja **criativo**! (Em caso de dúvida, peça orientação à CNIL).








