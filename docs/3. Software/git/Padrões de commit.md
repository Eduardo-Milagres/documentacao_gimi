# Padrões de commits 📜

De acordo com a documentação do **[Conventional Commits](https://www.conventionalcommits.org/pt-br)**, commits semânticos são uma convenção simples para ser utilizada nas mensagens de commit. Essa convenção define um conjunto de regras para criar um histórico de commit explícito, o que facilita a criação de ferramentas automatizadas.

Esses commits auxiliarão você e sua equipe a entenderem de forma facilitada quais alterações foram realizadas no trecho de código que foi commitado.

Essa identificação ocorre por meio de uma palavra e emoji que identifica se aquele commit realizado se trata de uma alteração de código, atualização de pacotes, documentação, alteração de visual, testee...

## Tipo e descrição 🦄

O commit semântico possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit ao utilizador(a) de seu código.

- `feat`- Commits do tipo feat indicam que a alteração está incluindo um **novo recurso** (se relaciona com o MINOR do versionamento semântico).

- `correção` - Commits do tipo correção indicam que seu arquivo commitado está **solucionando um problema** (bug correção), (se relaciona com o PATCH do versionamento semântico).

- `criação` - Commit do tipo criação indica que um novo arquivo foi criado.

- `docs` - Commits do tipo docs indicam que houveram **mudanças na documentação**, como por exemplo no Readme do seu repositório. (Não inclui alterações em arquivos).

- `teste` - Commits do tipo teste são utilizados quando são realizadas **alterações em testes**, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em arqiovos)

- `build` - Commits do tipo build são utilizados quando são realizadas modificações em **arquivos de build e dependências**.

- `perf` - Commits do tipo perf servem para identificar quaisquer alterações de arquivos que estejam relacionadas a **performance**.

- `refatoração` - Commits do tipo refatoração referem-se a mudanças devido a **refatorações que não alterem sua funcionalidade**, como por exemplo, uma alteração no formato como é processada determinada parte da peça, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a uma revisão.

- `tarefa` - Commits do tipo tarefa indicam **atualizações de tarefa** de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em arquivos)

- `ci` - Commits do tipo ci indicam mudanças relacionadas a **integração contínua** (_continuous integration_).

- `raw` - Commits to tipo raw indicam mudanças relacionadas a arquivos de configurações, dados, features, parametros.

- `remover` - Commits do tipo remover indicam a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado.

## Recomendações 🎉

- Adicione um tipo consistente com o título do conteúdo.
- Recomendamos que na primeira linha deve ter no máximo 4 palavras.
- Para descrever com detalhes, usar a descrição do commit.
- Usar um emoji no início da mensagem de commit representando sobre o commit.
- Os links precisam ser adicionados em sua forma mais autêntica, ou seja: sem encurtadores de link e links afiliados.

## Complementos de commits 💻

- **Rodapé:** informação sobre o revisor e número do card no Trello ou Jira. Exemplo: Reviewed-by: Elisandro Mello Refs #133
- **Corpo:** descrições mais precisas do que está contido no commit, apresentando impactos e os motivos pelos quais foram empregadas as alterações no arquivo, como também instruções essenciais para intervenções futuras. Exemplo: see the issue for details on typos correçãoed.
- **Descrições:** uma descrição sucinta da mudança. Exemplo: correção da legenda da peça.

## Padrões de emojis 💈

<table>
  <thead>
    <tr>
      <th>Tipo do commit</th>
      <th>Emoji</th>
      <th>Palavra-chave</th>
    </tr>
  </thead>
 <tbody>
     <tr>
      <td>Adição</td>
      <td>🆕 <code>:new:</code></td>
      <td><code>adição</code></td>
    </tr>
    <tr>
      <td>Alteração</td>
      <td>🔃 <code>:arrows_clockwise:</code></td>
      <td><code>alteração</code></td>
    </tr>
     <tr>
      <td>Criação</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>criação</code></td>
    </tr>
    <tr>
      <td>Correção</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>correção</code></td>
    </tr>
    <tr>
    <tr>
      <td>Salvamento</td>
      <td>💾 <code>:floppy_disk:</code></td>
      <td><code>correção</code></td>
    </tr>
    <tr>
      <td>Adicionando uma feature</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Removendo uma feature</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Liberação</td>
      <td>🚀 <code>:rocket:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Supressão/Visibilidade ativo</td>
      <td>⚫ <code>:black_circle:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Supressão/Visibilidade desativada</td>
      <td>⚪ <code>:white_circle:</code></td>
      <td></td>
    </tr>
    <tr>
        <td>Refatoração</td>
        <td>♻️ <code>:recycle:</code></td>
        <td><code>refatoração</code></td>
    </tr>
    <tr>
      <td>Limpeza de arquivo</td>
      <td>🧹 <code>:broom:</code></td>
      <td><code>limpeza</code></td>
    </tr>
    <tr>
      <td>Removerndo um arquivo</td>
      <td>🗑️ <code>:wastebasket:</code></td>
      <td><code>remover</code></td>
    </tr>
    <tr>
      <td>---</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>---</code></td>
    </tr>
    <tr>
      <td>Acessibilidade</td>
      <td>♿ <code>:wheelchair:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando um teste</td>
      <td>✅ <code>:white_check_mark:</code></td>
      <td><code>teste</code></td>
    </tr>
    <tr>
      <td>Atualizando a versão de um submódulo</td>
      <td>⬆️ <code>:arrow_up:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Retrocedendo a versão de um submódulo</td>
      <td>⬇️ <code>:arrow_down:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Alterações de revisão de arquivo</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Comentários</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Commit inicial</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>init</code></td>
    </tr>
    <tr>
      <td>Configuração</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>tarefa</code></td>
    </tr>
    <tr>
      <td>Documentação</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Em progresso</td>
      <td>🚧 <code>:construction:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Infraestrutura</td>
      <td>🧱 <code>:bricks:</code></td>
      <td><code>ci</code></td>
    </tr>
    <tr>
      <td>Lista de ideias (tasks)</td>
      <td>🔜 <code> :soon: </code></td>
      <td></td>
    </tr>
    <tr>
      <td>Mover/Renomear</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>tarefa</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
      <td>Revertendo mudanças</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>correção</code></td>
    </tr>
    <tr>
      <td>Tag de versão</td>
      <td>🔖 <code>:bookmark:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Teste de aprovação</td>
      <td>✔️ <code>:heavy_check_mark:</code></td>
      <td><code>teste</code></td>
    </tr>
    <tr>
      <td>Testes</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>teste</code></td>
    </tr>
    <tr>
      <td>Texto</td>
      <td>📝 <code>:pencil:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tratamento de erros</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td></td>
    </tr>
  </tbody>
</table>

## 💻 Exemplos

<table>
  <thead>
    <tr>
      <th>Comando Git</th>
      <th>Resultado no GitHub</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>git commit -m ":tada: Commit inicial"</code>
      </td>
      <td>🎉 Commit inicial</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":books: docs: Atualização do README"</code>
      </td>
      <td>📚 docs: Atualização do README</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bug: correção: Furação da base não coincide com furação do fechamento"</code>
      </td>
      <td>🐛 correção: Furação da base não coincide com furação do fechamento</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":sparkles: feat: Furação para luminária"</code>
      </td>
      <td>✨ feat: Furação para luminária</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":recycle: refatoração: Troca do furo feito em cut pelo furo com hole"</code>
      </td>
      <td>♻️ refatoração: Troca do furo feito em cut pelo furo com hole</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":zap: perf: Melhoria no tempo de resposta"</code>
      </td>
      <td>⚡ perf: Melhoria no tempo de resposta</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":boom: correção: Revertendo mudanças ineficientes"</code>
      </td>
      <td>💥 correção: Revertendo mudanças ineficientes</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":teste_tube: teste: Criando novo testee"</code>
      </td>
      <td>🧪 teste: Criando novo teste</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bulb: docs: Comentários sobre a peça X"</code>
      </td>
      <td>💡 docs: Comentários sobre a peça X</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":wastebasket: remover: removendo arquivos não utilizados do projeto para manter a organização e atualização contínua"</code>
      </td>
      <td>🗑️ remover: removerndo arquivos não utilizados do projeto para manter a organização e atualização contínua</td>
    </tr>
  </tbody>
</table>

# Principais comandos do Git 📜

- `git clone url-do-repositorio-no-github` - Clona um repositório remoto existente no GitHub para o seu ambiente local.

- `git init` - Inicializa um novo repositório Git no diretório atual.

- `git add .` - Adiciona todos os arquivos e alterações no diretório atual para a área de stage (preparando-os para o commit).

- `git commit -m "mensagem do commit"` - Registra as alterações adicionadas na área de stage com uma mensagem descritiva sobre o que foi modificado. 

- `git branch -M main` - Renomeia a branch atual (master) para main. O -M é usado para forçar a renomeação, movendo a branch se necessário.

- `git remote add origin https://github.com/usuario/nome-do-repositorio.git` - Adiciona um repositório remoto chamado origin ao repositório local. Use `https://github.com/usuario` para configurar o repositório remoto com HTTPS ou `git@github.com:usuario` para configurar com SSH.

- `git push -u origin main` - Envia os commits da branch main do repositório local para o repositório remoto origin e define main como a branch padrão para futuros push e pull. O -u (ou --set-upstream) configura a branch upstream para facilitar os próximos comandos git push e git pull e eliminar a necessidade de especificar a branch.

- `git remote add origin git@github.com:usuario/projeto.git` `git branch -M main` `git push -u origin main` - Quando você já tem um repositório local e quer conectá-lo a um repositório remoto no GitHub, adiciona o repositório remoto, renomeia a branch principal para main e envia os commits iniciais.

- `git fetch` - Busca todas as atualizações do repositório remoto sem integrá-las à branch atual. Isso atualiza as referências remotas.

- `git pull origin main`  - Atualiza a branch local main com as mudanças do repositório remoto origin. Combina git fetch e git merge.

- `git push --force-with-lease` - Forma mais segura de forçar o envio de alterações locais para o repositório remoto. Verifica se não houve alterações feitas por outros colaboradores desde sua última atualização local, evitando sobrescrever acidentalmente o trabalho de outros.

- `git revert id_do_commit_que_vai_ser_revertido` - Cria um novo commit que desfaz as alterações feitas pelo commit especificado, preservando o histórico. Útil para desfazer mudanças de forma segura sem reescrever o histórico.

- `git reset --hard id_do_commit_anterior_ao_que_vai_ser_apagado` - Redefine o repositório para o estado do commit especificado, apagando todas as mudanças feitas após esse commit. Ideal para uso local. Para sincronizar remotamente, use `git push --force-with-lease` posteriormente.

- `git commit --amend -m "mensagem_reescrita"` - Altera a mensagem do último commit. Após usar este comando, sincronize remotamente com `git push --force-with-lease`.

# Glossário 📖

- `fork` - Cópia de um repositório para a sua própria conta no GitHub. Isso cria um novo repositório em sua conta que é independente do original, permitindo que você faça alterações sem afetar o repositório original.

- `pull request` - Mecanismo usado para submeter alterações propostas ao repositório original. Um pull request é uma solicitação para que os mantenedores do projeto revisem e potencialmente incorporem as alterações. O pull request passará por um processo de avaliação e pode ser aceito ou rejeitado.

# Referência
Este arquivo foi copiado e modificado para atender necessidades internas, seguindo a referência do repositório [padrões de commit]({{ links.padroes_commit }}).
