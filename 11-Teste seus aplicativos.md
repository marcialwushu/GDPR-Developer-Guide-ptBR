# Sheet n°11: Teste seus aplicativos

#### O teste do seu produto permite verificar o funcionamento correto, garantir uma boa experiência do usuário e encontrar e evitar defeitos antes de entrar em produção. Testar seu produto também reduz o risco de violações de dados pessoais.

## Automatizar testes

* Os **testes de desenvolvimento** (unitários, funcionais etc.) verificarão a adequação entre as especificações e o funcionamento do produto. Os **testes de segurança** (testes aleatórios de dados também chamados "_fuzzing_", _scan_ de vulnerabilidades etc.) verificarão se o produto continua funcionando de maneira aceitável quando você se afasta do uso normal e se não apresenta nenhuma vulnerabilidade. isso poderia permitir que terceiros comprometessem sua segurança. Ambos os tipos de testes são importantes para o bom funcionamento do seu aplicativo.

* Configure um **sistema de integração contínua** para executar os testes automaticamente após cada alteração no seu código-fonte.

## Integre os testes à sua estratégia de negócios.


* Adicione a implementação do ambiente de teste à estratégia da empresa. As **métricas aceitáveis** devem ser definidas em conjunto por todas as partes antes do desenvolvimento.

* As métricas a serem consideradas são, por exemplo:

     * A **taxa de cobertura** dos testes e seu tipo;
     * a **taxa de duplicação** do seu código;
     * o **número de vulnerabilidades** (conforme definido pelas ferramentas) e seu tipo, etc.

## Cuidado com seus dados de teste!

* Dados de produção "reais" não devem ser usados durante a fase de desenvolvimento e teste. Usar dados pessoais do banco de dados de produção para fins de teste equivale a **desviá-los do seu objetivo original**.

* Se dados pessoais forem usados fora da produção, observe que os ** riscos à segurança **também aumentam**: acesso aos dados por pessoas que não precisam conhecer, vários locais de armazenamento, etc. .

* Portanto, crie um **conjunto de dados fictícios** que se parecerá com os dados que serão processados pelo seu aplicativo. Um conjunto de dados fictícios garantirá que a divulgação desses dados não tenha impacto nas pessoas.

* Se você precisar **importar configurações existentes** da produção para seus casos de teste, considere **anonimizar os dados pessoais** que possam estar presentes.
