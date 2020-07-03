#Git Códs Start

Este é um repositório de teste para estudo de como o git funciona e códs de fácil acesso para consultas

CONFIGS INICIAIS

git config —global user.name "SEU NOME"
git config —global [user.email](http://user.email) "SEU EMAIL"

git init // Inicializa o versionamento da pasta de trabalho

git add NOMEDOARQUIVO // Adiciona o arquivo a ser commitado
git add . // Adiciona todos os arquivos modificados a serem comitados

git commit -m "MENSAGEM DO ARQUIVO MODIFICADO"

LOGS

git log
git log —decorate
git log —autohor= "NOME"
git log shortlog // mostra todos os autores e seus commits
git shortlog -sn // mostra somente qtd de pessoas e qtd de commits

git diff // Visualiza a mudança no arquivo
git diff —name-only // Mostra apenas o nome do arquivo modificado

git show HASHDOCOMMIT

git checkout NOMEDOARQUIVO // Volta a uma ultima alteração

git reset HEAD NOMEDOARQUIVO // Remove o arquivo da fase de stage ( Já comitado )

git reset
—soft HASHDOARQUIVO
—mixed HASHDOARQUIVO
—hard HASHDOARQUIVO

CONFIGURANDO SSH NO GITHUB
Consute a documentação para maiores informações
https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

GERANDO A CHAVE EM SUA ESTAÇÃO DE TRABALHO
Abra o terminal e digite

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

As próximas fases pode digitar ENTER até finalizar o processo, caso queira uma maior segurança na pergunta pra adicionar uma senha, adicione uma senha a sua escolha.

Agora para ir ao diretório onde sua chave foi gerada digite

cd ~/.ssh/

Digite o comando para exibir sua chave que foi gerada

cat id_rsa.pub

Selecione a chave e copie, vá em settings na plataforma do github, clique em SSH and GPC keys, clique em New SSH key adicione o nome como titulo para poder identificar sua chave e cole sua chave. PRONTO, agora é só criar seus repositórios e trabalhar tranquilamente sabendo que seus projetos estão salvos e seguros.

Ainda não conhece ou não trabalha versionando seus projetos?
Acesse gratuitamente => https://www.udemy.com/course/git-e-github-para-iniciantes/

