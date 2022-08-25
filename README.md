# cmd-linux
Resumo de comandos do Linux 🐧



--Anotações para serem migradas

. shutdown <temp> > desliga o linux
. ip a > mostra a configuração de rede
. date > mostra a configuração da data
. 
. apt-get > executa a instalação/atualização de algum aplicativo
    - install
    - update
    - upgrade
. pwd > mostra o diretório que você está
. cd > troca de diretório (cd / )
    - / > vai para o diretório raiz
    - .. > retorna um diretório
    - <diretorio> vai para um diretório
    - quando montando um comando de acesso a algum diretório, se der um tab 2x, ele vai listar os dir/arquivos que tem dentro daquele diretório que está no comando de acesso 
. ls > lista os arquivos
    - | more > apresenta os arquivos de forma listada.
    Para cancelar a exibição, CTRL C
    - <nome arquivo/parte do nome do arquivo> para verificar se 
    o arquivo existe
    - <<parte do nome>*> > lista arquivos e diretórios com seus arquivos, aplicando o filtro
    - <? no nome do arquivo> substituir aquela letra por qualquer letra. Exemplo: ls g?o* irá listar arquivs que comecem com g, depois qualquer letra e depois o O e qualquer coisa no final...
. touch > para criar um arquivo
. find > utilizado para buscar um arquivo, a partir do diretório currente. 
    find -name arq*
. mkdir > para criar diretórios
. sudo > para rodar algo como administrador.
. cat > para visualizar informações de arquivos
. su > para acessar como super usuário (root)
. nano/vim para edição de arquivos.
. systemctl status <service> >> para verificar a situação de algum serviço
. history >> apresenta os útlimos 1000 comandos que foram utilizados recentemente.
    - history 30 > lista ios últimos 30
    - !<numero do comando> >> executa o comando com aquele número
    - !! executa o último comando
    - history | grep "Planilhas" >> vai buscar por exemplos os comandos que tiveram o nome planilhas
. | grep para efetuar alguma busca    
. chmod > para dar permissões
    - drwxrwxrwx
        . d > significa que aquele objeto é um diretório. Quando não tem o d, é um arquivo.
        . os próximos rwx > são a permissões do dono do arquivo
        . os rwx do meio são as permissões do grupo
        . os últimos rwx são as permissões dos outros
        d           rwx         rwx        rws
        dir/file    dono        grupo      outros
    - com base numérica, deve ser calculado qual permissão se deseja dar para cada grupo de permissão.
        Leitura(R)  4
        Gravacao(w) 2
        Execucao(x) 1
        Nenhuma     0
    - chmod 777 <dir/file> >> para dar permissão total aos 3 grupos
    - chmod 750 <dir/file>>> permissão total para o donom permissão de leitura e execução para o grupo que o proprietario pertence, nenhuma permissão para os demais.
. chown > para trocar o proprietário de um dir/file   
. apt-get > para manipular os pacotes nos linux
. apt >> versão mais amigável para gerenciar os pacotes
.fdisk > para criar partições no disco
.mkfs > para formatar a partição criadao. Deve ser informado qual o tipo de arquivo que desejo criar e qual disco.
.mount > para montar um disco no linux. mount /disco /dir
    . Para montar o disco automaticamente quando iniciar, deve ser adicionado a config no disco /etc/fstab.
        /disco  /dir que monta  /sistema arq    defaults 0 0
.umount > para desmontar o disco. Não perde as informações, só não lista mais.
. cp > para efetuar a copia de arquivos.
. mov > move arquivos
. mov > também é utilizado para renomear arquivos.
. ps > lista os processos que estão em execução para o usuário.
    - a > lista para todos os users
    - u > fornece o nome do user e a data
    - x > mostra os processos fora do console também
    - exemplo >> ls aux
. kill > para encerrar um processo.
    - killall <nome procesos> > para matar por nome de processo.
. w > mostra quem está logado
. who > mostra quem está logado com o pid para ser matado



Dicas
$ > no final do caminho do prompt indica que não está logado como super user
# > no final do caminho do prompt indica que está logado como super user.