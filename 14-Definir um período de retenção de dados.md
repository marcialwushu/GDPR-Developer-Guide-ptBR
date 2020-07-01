# Sheet n°14: Definir um período de retenção de dados

#### Os dados pessoais não podem ser mantidos por um período indeterminado: isso deve ser definido de acordo com os propósitos do processamento. Uma vez alcançado esse objetivo, os dados devem ser arquivados, excluídos ou tornados anônimos (por exemplo, para produzir estatísticas).

## Ciclos de retenção de dados

* O ciclo de retenção de dados pessoais pode ser dividido em **três fases sucessivas distintas**:
     * O banco de dados ativo;
     * Arquivamento intermediário;
     * Arquivamento final ou exclusão.


* Os mecanismos para excluir dados pessoais das bases ativas garantem que os dados sejam mantidos e acessíveis apenas pelos serviços operacionais **pelo tempo necessário para atingir o objetivo da operação de processamento**.

* Verifique se **os dados não são mantidos nos bancos de dados ativos** simplesmente observando-os **como sendo arquivados**. Os dados arquivados (arquivo intermediário) devem estar acessíveis apenas a um serviço específico responsável por acessá-los e removê-los do arquivo, se necessário.

* Verifique também se você possui **modos de acesso especificados** para os dados arquivados, pois o uso de um arquivo deve ser ad hoc e excepcional.

* Se possível, use a mesma implementação ao implementar a **remoção de dados ou anonimato** que aquela que gerencia o **direito de exclusão** (consulte [folha sobre o exercício dos direitos](Sheet_n°13:_Prepare_for_the_exercise_of_people's_rights) ), para garantir uma operação homogênea do seu sistema.

## Alguns exemplos de prazo de validade

* Os **dados relativos ao gerenciamento da folha de pagamento ou ao controle do tempo dos funcionários** podem ser mantidos por 5 anos.

* Os **dados em um arquivo médico** devem ser mantidos por 20 anos.

* Os **dados de um possível cliente que não responde a nenhuma solicitação** podem ser mantidos por 3 anos.

* Os **dados de log** podem ser mantidos por 6 meses.

