# Sheet n°3: Protegendo seu ambiente de desenvolvimento

#### A segurança dos servidores de produção, desenvolvimento e integração contínua, bem como as estações de trabalho do desenvolvedor, devem ser uma prioridade, pois centralizam o acesso a uma grande quantidade de dados.

## Avalie seus riscos e adote as medidas de segurança apropriadas

* **Avalie os riscos** nas ferramentas e processos usados para seus desenvolvimentos. Faça um inventário de suas medidas de segurança existentes e defina um plano de ação para melhorar sua cobertura de riscos. Nomeie uma pessoa responsável por sua implementação.

* Considere os riscos de todas as ferramentas usadas, incluindo os riscos relacionados ao SaaS (Software como Serviço) e ferramentas colaborativas na nuvem (como [Slack](https://slack.com), [Trello](https: //trello.com), [GitHub](https://github.com) etc.).

## Proteja seus servidores e estações de trabalho de maneira homogênea e reproduzível

* As listas de **recomendações** relativas à segurança de servidores, estações de trabalho e redes internas estão disponíveis nas [sheets  n ° 5 a 8](https://www.cnil.fr/sites/default/files/atoms/files /cnil_guide_securite_personnelle_gb_web.pdf) do **guia de segurança de dados pessoais** do CNIL.

* Escreva um **documento listando essas medidas e explicando sua configuração** para garantir que as medidas de segurança sejam implementadas uniformemente em servidores e estações de trabalho. Para reduzir a carga de trabalho, **ferramentas de gerenciamento de configuração**, como [Ansible](https://github.com/ansible/ansible), [Puppet](https://github.com/puppetlabs/puppet) ou [Chef](https://github.com/chef/chef), pode ser usado.

* Atualize servidores e estações de trabalho, se possível automaticamente. Você pode configurar uma lista de observação das vulnerabilidades mais importantes, por exemplo, os [NVD Data Feeds](https://nvd.nist.gov/vuln/data-feeds).

## Ênfase especial no gerenciamento de acesso e na rastreabilidade das operações

* Lembre-se de documentar o gerenciamento de suas **chaves SSH** (uso de criptografia de última geração e algoritmos de comprimento de chave, proteção de chaves privadas com uma senha, rotação de chaves). Para exemplos de boas práticas, consulte [o documento sobre o uso seguro do SSH (aberto)](https://www.ssi.gouv.fr/uploads/2014/01/NT_OpenSSH_en.pdf).

* Incentive uma autenticação forte nos serviços usados pela equipe de desenvolvimento.

* **Rastreie** o acesso às suas máquinas e, se possível, implemente **análise de log automatizada**. Para manter rastreamentos confiáveis, o uso de contas genéricas deve ser evitado.


