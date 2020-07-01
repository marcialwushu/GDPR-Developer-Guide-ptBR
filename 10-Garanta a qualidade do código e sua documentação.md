# Sheet n°10: Garanta a qualidade do código e sua documentação

#### É essencial adotar boas técnicas de escrita de código o mais rápido possível. A legibilidade do código reduz o esforço de manutenção e correções de bugs ao longo do tempo para você e seus (possivelmente futuros) colaboradores.

## Código e arquitetura do documento

* Às vezes, a documentação é deixada de fora durante o desenvolvimento, devido à falta de tempo ou visibilidade do projeto. No entanto, é **crucial para a manutenção do seu projeto**: permite entender como o código funciona globalmente e saber quais partes do código são afetadas por uma modificação.

* **Documente a arquitetura, não apenas o código**: você precisa manter a visão geral em mente ao escrever sua documentação e ajudar os desenvolvedores a entender como todos os seus componentes funcionam juntos. Portanto, concentre-se em diagramas e explicações claras ao documentar seu projeto.

* **Mantenha a documentação juntamente com o código**: A melhor maneira de manter sua documentação atualizada é modificá-la à medida que avança no código.

* Se você usa um gerenciador de código-fonte, também pode incluir alterações na documentação para cada "_commit_" que modifica seu código (consulte em particular [o formulário "Gerenciar seu código-fonte"]](#Sheet_n°4_:_Gerenciar_seu_código-fonte)).

* **Não se esqueça de abordar a segurança na sua documentação**. Em particular, você pode documentar as diferentes opções de configuração para seu aplicativo e explicar quais configurações são as mais seguras.

## Verifique a qualidade do seu código e sua documentação.

* Um código de qualidade envolve **adoção de boas práticas e convenções de codificação** aplicadas de forma consistente ao longo do programa. Também é melhor consultar as [convenções existentes](https://github.com/Kristories/awesome-guidelines). Aqui estão alguns exemplos de boas práticas:
     * **O uso explícito de nomes de variáveis e funções** facilita a compreensão do que está acontecendo à primeira vista.
     * **Recuar corretamente seu código** permite que você veja a estrutura do código mais rapidamente.
     * **Evitar redundância de código** reduz os esforços de correção que precisam ser feitos em vários locais. Um descuido é rapidamente esquecido.
     
* **As ferramentas podem ajudá-lo a controlar a qualidade do seu código**. Uma vez configurados corretamente, eles evitarão reler o código para verificar a implementação correta das convenções de codificação. Exemplos dessas ferramentas são:

     * **Ambientes de desenvolvimento integrados** ("_IDE_"), possivelmente usando plugins ("_plugins_"), podem ser configurados para respeitar as regras de indentação de código, quebras de linha entre diferentes partes do código ou a posição de chaves e outros parênteses.
     * **O software de medição da qualidade do código fonte** pode relatar duplicações de código, conformidade com regras de programação ou possíveis bugs.     

