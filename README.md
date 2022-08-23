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


Dicas
$ > no final do caminho do prompt indica que não está logado como super user
# > no final do caminho do prompt indica que está logado como super user.