# gitcommands
Some git commands, still need improvements

git init -> iniciar um repositório no git.

git add - > mudar o arquivo do estado Untracked para Staged.

git status -> checa estados dos files.

git commit -> commitar.

git remote add origin <linkDoRepositorio> - > enviar files do local para o remoto.
  
git remote -v -> listar os repositórios remotos registrados.
  
git clone linkDoRepositorio -> clonar repositório remoto para utilizar localmente.
  
git push origin <branch> -> empurrar para o repositório remoto pela branch informada.
  
git pull -> puxar info do repositório remoto para o local.
  
git pull origin <branch> -> puxar do repo local pela branch informada.
  
git branch -> mostra as branches e a branch que está ativa.
  
git checkout -b nomeDaNovaBranch -> se movimentando entre as branches e criando uma nova branch simultaneamente.
  
git checkout nomeDaBranch -> volta a apontar para branch com nome utilizado no comando.
  
git brach -m novoNome -> para mudar nome da branch que esta utilizando
  
git checkout main -> ir para branch main
  
git branch -m nomeBranchAntiga -> mover para branch main 
  
git branch -m nomeBranchAntiga  nomeBranchNova -> mudar nome de uma branch para outra
  
git branch -d branchQueQuerDeletar -> deletar uma branch
  
git merge nomeBranch -> as branches irão apontar para a mesma HEAD
  
git stash save “mensagem” -> pega tudo que está no staged área e adiciona numa caixa, como se fosse um array, você pode adicionar vários stashes.
  
git stash list -> vai mostrar o índice do stash, qual branch esta e a mensagem com a descrição da modificação.
Ex: stash@{0}: On <branchName>: <mensagemDescricaoDaMudanca>  ->> não vai aparecer no git status como pendente, pois está guardado.
  
git stash -> checa se há diretório de trabalho salvo e indexado com o estado de WIP(work in progress) on <branch>:
  
git stash pop 1(indiceDaAlteração) -> abrir a “caixa” onde estava guardada as info no stash, neste caso no índice 1.
  
git stash clear -> apagar tudo que estiver no stash.
  
git log -> ver o log
  
git log <nomeDiretorio> -> para ver log de um determinado diretório
  
git log <nomeFile> -> para ver logo de um determinado arquivo
  
git log –oneline -> histórico de commits de forma reduzida
 
git log - - graph -> mostra de maneira gráfica, simples, o log das movimentações
  
gitk -> abre ferramenta gráfica mostrando, de maneira gráfica e lista mais detalhada, as movimentações
  
git reset hash ou HEAD -> com hash revertando aquele commit especifico que  pertence a hash, HEAD reseta para o ultimo commit valido naquela arvore.
  
git reset hashCode
  
git reset HEAD~1 -> Reseta numero utilizado após o sinal de til em commit com HEAD
  
git reset -- soft -> rever o commit ainda sem fazer o push, ou seja, que está em branch main, de volta para o staging/index área, 
como se estivesse adicionado mas não commitado ainda.

git reset - - mixed -> move de volta para o working directory, como se ainda não estivessem adicionados.
  
git reset - - hard -> 
  
git revert HEAD~1 -> Vai gerar um commit novo com o inverso.
  
git config –global core.editor “code –wait” -> setar editor de texto padrão, nesse caso, o vs code.
  
git config –global –list -> listar as configurações globais
  
git config –global –unset core.editor -> retirar as configurações setadas do editor de texto padrao
