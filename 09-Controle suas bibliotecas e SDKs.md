# Sheet n°09: Controle suas bibliotecas e SDKs

#### Você usa bibliotecas, SDKs ou outros componentes de software criados por terceiros? Aqui estão algumas dicas sobre como integrar essas ferramentas, mantendo o controle de seus desenvolvimentos.

## Faça uma escolha informada

* **Avalie o valor da adição de cada dependência.** Alguns tijolos de software comumente usados têm apenas algumas linhas. No entanto, cada elemento adicionado é um aumento na superfície de ataque do seu sistema. No caso em que uma única biblioteca oferece várias funcionalidades, integre apenas as funcionalidades que você realmente precisa. Ao ativar o número mínimo de funcionalidades, você reduz o número de possíveis erros que podem ocorrer.

* **Escolha software, bibliotecas e SDKs mantidos:**

     * Se você deseja usar software livre ou de código aberto, tente escolher projetos ou soluções com uma comunidade ativa, atualizações regulares e boa documentação.

     * Se você usar outros tipos de soluções com suporte comercial, garanta contratualmente que o código seja mantido e atualizado por toda a vida útil do seu projeto.

* **Leve em consideração a privacidade.** Alguns SDKs ou bibliotecas se pagam usando dados pessoais coletados dos aplicativos ou sites nos quais estão integrados. Certifique-se de que esses terceiros cumpram as leis aplicáveis em relação aos dados pessoais, incluindo um mecanismo para obter o consentimento do usuário.

* **Se você usar mecanismos criptográficos, é altamente desencorajado implementar os algoritmos ou protocolos criptográficos**, mas tente escolher as bibliotecas criptográficas mantidas, reconhecidas e fáceis de usar.

## Avalie os elementos selecionados

* **Leia a documentação e altere as configurações padrão**. É importante saber como suas dependências funcionam. Bibliotecas e SDKs de terceiros geralmente vêm com arquivos de configuração padrão, que raramente são alterados devido à falta de tempo, o que causa muitas falhas de segurança.
* **Audite suas bibliotecas e SDKs.** Você realmente sabe o que todas as bibliotecas e SDKs integrados fazem? Quais dados são enviados por essas dependências e para quem? Essa auditoria permitirá determinar as obrigações de proteção de dados a serem respeitadas e estabelecer a responsabilidade dos atores.
* **Mapeie suas dependências.** As bibliotecas e SDKs de terceiros também podem integrar outros componentes: a auditoria de seu código permitirá mapear melhor todas as suas dependências e agir melhor se um problema afetar uma delas. Também é recomendável que você execute auditorias de segurança de seus componentes de terceiros e os monitore.
* **Cuidado com o [typosquatting](https://en.wikipedia.org/wiki/Typosquatting) e outras técnicas maliciosas.** Verifique os nomes das dependências e suas próprias dependências para evitar ataques. Não copie e cole linhas de comando de sites desconhecidos.

## Manter bibliotecas e SDKs

* **Use sistemas de gerenciamento de dependências** (como yum, apt, maven, pip, etc.) para manter uma lista atualizada de suas dependências.
* **Gerencie atualizações para suas dependências,** especialmente no caso de atualizações de segurança que corrigem vulnerabilidades. Você deve configurar um procedimento documentado para gerenciar e implantá-los o mais rápido possível.
* **Esteja ciente das versões de bibliotecas e SDKs no final do suporte** que não serão mais mantidas: tente encontrar outra solução (escolha uma nova biblioteca, renove o suporte comercial).
* **Verifique o status dos projetos de código aberto,** especialmente a mudança de domínio ou propriedade de pacote, alguns ataques usando atualizações maliciosas de dependências populares.

     
