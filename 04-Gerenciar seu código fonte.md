# Sheet n°4: Gerenciar seu código fonte

#### Qualquer que seja o tamanho do seu projeto, é altamente recomendável usar uma ferramenta de gerenciamento de código fonte, como um * sistema de controle de versão *, para rastrear suas diferentes versões ao longo do tempo.

Configure seu sistema de controle de versão com eficiência, pensando em sua segurança.

* Um sistema de controle de versão é um programa de software que permite armazenar **todo o seu código-fonte e arquivos associados**, mantendo a **cronologia de todas as alterações** que foram feitas. Um servidor FTP simples não é um sistema de controle de versão.

* Configure seu ambiente corretamente usando os recursos oferecidos pelo seu sistema de controle de versão. É recomendável que você implemente forte **autenticação** e / ou **autenticação com chaves SSH** no início do seu projeto.

* Além disso, atribua *níveis de acesso* ao seu projeto aos usuários do seu sistema de controle de versão e defina para cada nível as **permissões** correspondentes (por exemplo, um nível "convidado" com direitos de leitura limitados, um "desenvolvedor" "nível com direitos de gravação etc.).

* Faça **backups** regulares do seu sistema de gerenciamento de código-fonte. Lembre-se de fazer backup do servidor principal, onde todas as alterações são salvas.

* Estabeleça procedimentos de desenvolvimento para trabalhar com eficiência, mesmo que **várias pessoas estejam desenvolvendo ao mesmo tempo**. Por exemplo, você pode decidir não trabalhar na mesma ramificação (_master_), mas configurar ramificações baseadas em recursos, que serão mescladas na ramificação principal à medida que o desenvolvimento avança. Tais estratégias de desenvolvimento já estão bem documentadas, por exemplo, em [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/). Além disso, alguns sistemas de controle de versão oferecem a configuração de **ramificações protegidas** que impedem alterações não autorizadas nos arquivos nessas ramificações.

## Esteja ciente do seu conteúdo de código-fonte.


* Implemente **ferramentas de métricas de qualidade de código** que varrerão seu código assim que for _commitido_ para verificar sua boa qualidade. Você também pode adicionar scripts para verificar essas métricas na [configuração do sistema de controle de versão](https://git-scm.com/book/uz/v2/Customizing-Git-Git-Hooks): o _commit_ será cancelado se o o código fonte não é de qualidade suficiente.

* Mantenha seus segredos e senhas fora do seu repositório de código-fonte:
     * em arquivos **separados, que não foram _comprometidos _**. Lembre-se de usar arquivos especiais do seu sistema de controle de versão (como _.gitignore_ para _Git_) para que você não confirme arquivos confidenciais por engano.
     * em **variáveis de ambiente**, verifique se as variáveis de ambiente não são gravadas acidentalmente em *logs* ou exibidas quando ocorre um erro de aplicativo.
     * usando [**software específico de gerenciamento de secrets ou configuração**](https://www.digitalocean.com/community/tutorials/an-introduction-to-managing-secrets-safely-with-version-control-systems#using-configuration-management-systems-for-secret-management).
     
Finalmente, se você precisar incluir esses dados em seu repositório, considere **criptografar/descriptografar automaticamente** os arquivos usando um *plugin* do seu sistema de controle de versão (por exemplo, [_git-crypt_](https://github.com/AGWA/git-crypt)).

* Após um _commit_ que contém dados pessoais ou outros dados críticos, não se esqueça de [limpar](https://git-scm.com/book/en/v2/Git-Tools-Rewriting-History) [completamente](https : //help.github.com/en/github/authenticating-to-github/removing-sensitive-data-from-a-repository#purging-a-file-from-your-repositorys-history) o repositório do código-fonte: mesmo após a modificação, os dados ainda podem estar disponíveis no histórico do seu repositório.

* Tenha cuidado antes de **publicar seu código fonte online**. Revise **todo o seu conteúdo** para garantir que não haja dados pessoais, senhas ou outros segredos, incluindo todo o histórico de alterações.

## Exemplos de ferramentas

* Diferente de ferramentas como [Subversion](https://subversion.apache.org/), que precisam de um servidor central para serem executadas, os principais sistemas de controle de versão ([Git](https://git-scm.com/) , [Mercurial](https://www.mercurial-scm.org/) por exemplo) são **descentralizados**.

* Para a maioria dessas ferramentas, é fornecida uma **interface da web e ferramentas relacionadas** (gerenciamento de bugs, wiki para sua documentação etc.). Essas soluções podem ser acessíveis via Internet ([GitHub](https://github.com/), [Bitbucket](https://bitbucket.org/) etc.) ou podem ser integradas à sua própria conta. servidores.





