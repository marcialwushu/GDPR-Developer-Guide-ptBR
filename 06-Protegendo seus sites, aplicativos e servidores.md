# Sheet n°6: Protegendo seus sites, aplicativos e servidores

#### Qualquer site, aplicativo ou servidor deve incorporar regras básicas de segurança de ponta, não apenas nas comunicações em rede, mas também na autenticação e infraestrutura.

## Protegendo redes de comunicação

* **Implemente o TLS versão 1.2 ou 1.3** (substituindo SSL) em todos os sites e para transmissão de dados de seus aplicativos móveis, por exemplo, com [LetsEncrypt](https://letsencrypt.org/fr/), usando apenas os versões recentes e verificação de sua correta implementação.

* **Torne obrigatório o uso do TLS** para todas as páginas do seu site e para seus aplicativos móveis.

* **Limite as portas de comunicação** estritamente necessárias para o bom funcionamento dos aplicativos instalados. Se o acesso a um servidor Web for possível apenas usando o protocolo HTTPS, apenas as portas 443 e 80 deste servidor deverão estar acessíveis, todas as outras portas poderão ser bloqueadas pelo firewall.

* **A OWASP publicou em seu site algumas dicas** por exemplo, para [implementar corretamente o TLS](https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html) ou para [proteger um serviço da web](https://cheatsheetseries.owasp.org/cheatsheets/Web_Service_Security_Cheat_Sheet.html).

## Protegendo autenticações

* **Siga [a recomendação da CNIL sobre senhas](https://www.cnil.fr/fr/node/23803)**. Lembre-se de limitar o número de tentativas de acesso.

* **Nunca armazene senhas em texto não criptografado**. Armazene-os como um hash usando uma biblioteca comprovada, como [bcrypt](https://en.wikipedia.org/wiki/Bcrypt).

* **Se forem utilizados cookies para autenticação**, é recomendável:

     * para forçar o uso de HTTPS via [HSTS](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security);

     * para usar a flag `secure`;

     * use a flag `HttpOnly`.

* **Teste os conjuntos criptográficos instalados nos sistemas** e desative os obsoletos (RC4, MD4, MD5 etc.). Incentive o uso do AES256. [Leia a nota do OSWAP sobre o assunto](https://owasp.org/www-project-cheat-sheets/cheatsheets/Cryptographic_Storage_Cheat_Sheet.html).

* **Adote uma política de senha específica para administradores**. Altere as senhas, pelo menos, sempre que um administrador sair e em caso de suspeita de violação. Incentive a autenticação forte quando possível.

* **Limite o acesso a ferramentas e interfaces de administração a equipe qualificada.** Incentive o uso de contas com privilégios mais baixos nas operações diárias.

* **O acesso remoto às interfaces de administração deve estar sujeito a maiores medidas de segurança.** Por exemplo, para servidores internos, a implementação de uma VPN com autenticação forte do usuário e da estação de trabalho que ele está usando pode ser uma boa solução.


## Protegendo infraestruturas

* **Faça backups, se possível, criptografados e verificados regularmente**. Isso é especialmente útil no caso de um ataque de ransomware nos seus sistemas, pois ter backups para todos os seus sistemas será a única medida que permitirá restaurar seus sistemas.

* **Limite o tamanho da pilha de software usada,** e para cada elemento da pilha:

     * **Instale atualizações críticas** sem demora, agendando uma verificação semanal automática;
     * **Automatize uma verificação de vulnerabilidades**, assinando o [NVD Data Feeds](https://nvd.nist.gov/vuln/data-feeds), por exemplo.
     
* **Use ferramentas de detecção de vulnerabilidade** para os processos mais críticos para detectar possíveis violações de segurança. Sistemas para detectar e prevenir ataques a sistemas ou servidores críticos também podem ser usados. Esses testes devem ser realizados regularmente e antes que qualquer nova versão de software seja colocada em produção.

* **Restrinja ou proíba o acesso físico e de software às portas de diagnóstico e configuração remota.** Por exemplo, você pode listar todas as portas abertas usando a ferramenta * netstat *.

* **Proteja os bancos de dados que você disponibiliza na Internet**, pelo menos restringindo o acesso o máximo possível (por exemplo, por filtragem de IP) e alterando a senha padrão da conta de administrador.

* Em termos de gerenciamento de banco de dados, boas práticas incluem:

     * **usando contas nominativas** para acesso ao banco de dados e crie contas específicas para cada aplicativo;
     * **revogando os privilégios administrativos** das contas de usuário ou aplicativo para evitar modificações na estrutura do banco de dados (tabela, valores, processo, etc);
     * ter proteção contra ataques de injeção de SQL ou script;
     * encorajamento em repouso e criptografia de disco e banco de dados.
     
     


