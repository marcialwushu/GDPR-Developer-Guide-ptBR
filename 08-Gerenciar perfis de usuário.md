# Sheet n°8: Gerenciar perfis de usuário

#### A maneira de gerenciar perfis de seus colaboradores e usuários finais deve ser pensada antes dos seus desenvolvimentos. Consiste em definir diferentes perfis de acesso e autorização para que cada pessoa possa acessar apenas os dados de que realmente precisa.


## Boas práticas para gerenciamento de usuários

* Tudo começa com o **uso de identificadores únicos e individuais**, sejam eles usuários de seu aplicativo ou colaboradores no desenvolvimento.

* Certifique-se de **impor autenticação** antes de qualquer acesso aos dados pessoais, de acordo com as [recomendações da CNIL](https://www.cnil.fr/en/passwords-minimum-security-recommendations-businesses- e cidadãos).

* Para garantir que cada pessoa (usuário ou colaborador) possa acessar apenas **dados de que ele realmente precisa**, seu sistema deve fornecer **políticas diferenciadas de gerenciamento de acesso a dados** (ler, gravar, excluir etc.) de acordo com para pessoas e necessidades. Um mecanismo global de gerenciamento de perfil de usuário permitirá agrupar direitos diferentes de acordo com uma função exercida por um grupo de usuários no aplicativo.

* O gerenciamento de perfis de usuário pode ser usado juntamente com **sistemas de registro para rastrear atividades e detectar anomalias ou eventos relacionados à segurança**, como acesso fraudulento e uso indevido de dados pessoais. Esses dispositivos não devem ser utilizados para nenhuma outra finalidade que não seja garantir o uso adequado do sistema de computador. Os logs também não devem ser mantidos por mais tempo que o necessário. Em geral, um período de seis meses é adequado.

* Você também pode planejar auditorias de código ou testes de penetração em seu ambiente de desenvolvimento para **garantir a robustez do seu sistema de gerenciamento de perfis**.

## Simplifique o gerenciamento de perfis de liberação

* Planeje **documentar ou automatizar o movimento de seus colaboradores**. Por exemplo, esses procedimentos devem levar as ações a serem tomadas quando as pessoas não estiverem mais autorizadas a acessar uma sala ou recurso de TI ou no final de seu contrato.

* Gerenciar seus usuários e colaboradores implica **uma revisão regular da permissão** de acordo com a evolução dos usos e movimentos organizacionais dentro do seu projeto. O uso de serviços de diretório, como o _LDAP_, ajudará você a monitorar essas alterações e a refinar suas estratégias de acesso, por exemplo, atribuindo funções com base nos perfis de uso. Isso permite que você respeite melhor o princípio do menor privilégio.


* O uso de contas "supremas" (tipo _root_, administrador etc.) deve ser evitado para operações convencionais, pois constitui a pedra angular do seu sistema e um destino privilegiado para um possível invasor externo. Recomendamos que você associe uma política de senha forte a ela (10 a 20 caracteres ou multifator) e limite o número de pessoas com conhecimento dela ao estritamente necessário.


* **Favorecer o uso de um gerenciador de senhas no seu projeto** e a transição para autenticação forte, quando possível. Evite contas genéricas compartilhadas por várias pessoas.

