  - Gustavo da Silva Ribeiro
     - Nascimento: 27/07/1999
      - Lindo da Mamãe

     - Esta atividade tem como objetivo demonstrar e praticar os fundamentos do fluxo de trabalho com Git e GitHub. 
 Ela abrange desde a inicialização de um repositório remoto e local até as operações básicas de adição, commit,
envio de alterações, criação e troca de branches, e finalmente, a integração dessas branches. 
 A necessidade de registrar cada operação com um printscreen
reforça a importância de documentar o processo e visualizar as mudanças no seu terminal ou interface gráfica do Git.

     - A lista de comandos Git utilizados (com explicação)


 -git init
 Explicação: Inicializa um novo repositório Git local no diretório atual. Este comando cria um subdiretório .git onde o Git
 armazena todos os metadados e o histórico do repositório. Você geralmente executa este comando apenas uma vez por projeto.

 -git clone <URL_do_repositório>:
 Explicação: Cria uma cópia local de um repositório Git que já existe remotamente (por exemplo, no GitHub).
 O <URL_do_repositório> é o endereço web do repositório remoto. Este comando baixa todos os arquivos, o histórico
 completo e as branches do repositório remoto para a sua máquina local.

 -git status:
 Explicação: Exibe o estado do seu diretório de trabalho e da área de staging. Ele mostra quais arquivos foram modificados, 
quais estão na área de staging (prontos para o commit) e quais arquivos não estão sendo rastreados pelo Git. É um comando útil para verificar
 o status das suas alterações antes de realizar um commit.

 -git add <arquivo(s)>:
Explicação: Adiciona as alterações feitas nos <arquivo(s)> à área de staging. Isso significa que o Git irá incluir essas alterações no próximo commit.
 Você pode usar git add . para adicionar todas as alterações no diretório atual e seus subdiretórios, ou especificar arquivos individuais 
(por exemplo, git add index.html README.txt).

 -git commit -m "<mensagem do commit>":
 Explicação: Registra as alterações que estão na área de staging no histórico do repositório local. A <mensagem do commit> é uma descrição concisa
 das alterações que você está incluindo neste commit. Boas mensagens de commit são importantes para entender o histórico do projeto. A flag -m permite
 que você escreva a mensagem diretamente na linha de comando.

 -git push <remoto> <branch>:
 Explicação: Envia os commits do seu repositório local para um repositório remoto. <remoto> é o nome da conexão com o repositório remoto
 (geralmente origin para o repositório clonado do GitHub), e <branch> é o nome da branch local que você deseja enviar (geralmente main ou master). 
Este comando sincroniza o seu trabalho local com o repositório remoto, tornando suas alterações visíveis para outros colaboradores.

 -git branch:
 Explicação: Lista todas as branches existentes no seu repositório local. A branch atualmente ativa é geralmente marcada com um asterisco (*).
git branch <nome_da_branch>:
 .Explicação: Cria uma nova branch local com o <nome_da_branch> especificado. Este comando apenas cria a branch; você ainda precisa mudar para ela usando o git checkout.
git checkout <nome_da_branch>:

 .Explicação: Muda a sua branch ativa para a <nome_da_branch> especificada. Isso move o seu diretório de trabalho para o estado da branch que você escolheu, permitindo que você trabalhe isoladamente nessa branch.
git merge <branch_a_ser_incorporada>:

.Explicação: Integra as alterações da <branch_a_ser_incorporada> na branch atualmente ativa. Por exemplo, se você estiver na branch main e executar git merge desenvolvimento, as alterações da branch desenvolvimento serão incorporadas à sua branch main. O Git tentará fazer isso automaticamente, mas pode haver conflitos que precisam ser resolvidos manualmente.
