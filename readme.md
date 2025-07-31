Projeto de Exemplo com GIT

GIT boas praticas – histórico.
GIThub – repositório.

Chave public
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIGAsZ+amvDEPUEgwKcqHT8NOcqn8lrFFfNMrmMGak7TF rbrtooliveira@gmail.com

ir na conta, setting-ssh and gpg Keys.

Add nova chave ssh.
Ir no repositório em ssh . copiar e ir para o terminal.

Verificar branch
Git checkout

Git checkout –b feature/files

Mudar de branch – git checkout nome da branch.

Verificar a branch – git branch

Enviar branch.
Git push –set-upstream origin “nome”.

Solução segura (recomendada): primeiro puxe as alterações remotas
bash
CopiarEditar
git pull origin develop --rebase
Depois, tente novamente:
bash
CopiarEditar
git push origin develop
O --rebase vai tentar aplicar seus commits locais por cima dos que estão no servidor, evitando um merge commit desnecessário.
Git pull traz as mudança para a maquina.

