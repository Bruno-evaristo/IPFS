Instalação do IPFS:

Pode fazer o Download: https://ipfs.io/ipns/dist.ipfs.io/go-ipfs

Extraia o arquivo: tar xvfz <nome do arquivo> tar.gz

 \\Sobre mover o arquivo existem dois modos:

1- Pode ser feito de forma manual:

     movendo o arquivo ipfs para /usr/local/bin/ipfs

2- ou através do terminal de comando:

     cd go-ipfs/
     mv ipfs

 \\para o caminho
     /usr/local/bin/ipfs

---------------------------------------------------------------------------------------------------

Iniciando o IPFS e suas Informações básicas:

 \\Primeiramente verifique a versão e se o ipfs está de fato instalado através dos comandos:

        ifps help

 \\deverá ter como resposta a mensagem;

USAGE:

    ipfs - global p2p merkle-dag filesystem

    ipfs [<flags>] <command> [<arg>] ...

    BASIC COMMANDS
    
        init          Initialize ipfs local configuration
        add <path>    Add an object to ipfs
        cat <ref>     Show ipfs object data
        get <ref>     Download ipfs objects
        ls <ref>      List links from an object
        refs <ref>    List hashes of links from an object
    
    DATA STRUCTURE COMMANDS
    
        block         Interact with raw blocks in the datastore
        object        Interact with raw dag nodes
        file          Interact with Unix filesystem objects
    
    ADVANCED COMMANDS
    
        daemon        Start a long-running daemon process
        mount         Mount an ipfs read-only mountpoint
        resolve       Resolve any type of name
        name          Publish or resolve IPNS names
        dns           Resolve DNS links
        pin           Pin objects to local storage
        repo gc       Garbage collect unpinned objects
    
    NETWORK COMMANDS
    
        id            Show info about ipfs peers
        bootstrap     Add or remove bootstrap peers
        swarm         Manage connections to the p2p network
        dht           Query the dht for values or peers
        ping          Measure the latency of a connection
        diag          Print diagnostics
    
    TOOL COMMANDS
    
        config        Manage configuration
        version       Show ipfs version information
        update        Download and apply go-ipfs updates
        commands      List all available commands
    
    Use 'ipfs <command> --help' to learn more about each command.


*Agora o usuário possui o IPFS instalado e funcionando no computador.


 \\O usuário pode verificar a versão e o local que o arquivo ipfs está instalado:

       ipfs version
       which ipfs

 \\Iniciar o IPFS:

       ipfs init


Terá como resultado:
 
initializing ipfs node at /Users/jbenet/.go-ipfs
generating 2048-bit RSA keypair...done
peer identity: Qmcpo2iLBikrdf1d6QU6vXuNb6P7hwrbNPW9kLAH8eG67z
to get started, enter:

         ipfs cat /ipfs/QmYwAPJzv5CZsnA625s3Xf2nemtYgPpHdWEz79ojWnPbdG/readme

Será gerado gerado um Hash do Usuário, que será utilizado da seguinte forma:

         ipfs cat /ipfs/QmYwAPJzv5CZsnA625s3Xf2nemtYgPpHdWEz79ojWnPbdG/readme


 \\Deverá ter como resultado:


Hello and Welcome to IPFS!

██╗██████╗ ███████╗███████╗
██║██╔══██╗██╔════╝██╔════╝
██║██████╔╝█████╗  ███████╗
██║██╔═══╝ ██╔══╝  ╚════██║
██║██║     ██║     ███████║
╚═╝╚═╝     ╚═╝     ╚══════╝

If you're seeing this, you have successfully installed
IPFS and are now interfacing with the ipfs merkledag!

 -------------------------------------------------------
| Warning:                                              |
|   This is alpha software. use at your own discretion! |
|   Much is missing or lacking polish. There are bugs.  |
|   Not yet secure. Read the security notes for more.   |
 -------------------------------------------------------

Check out some of the other files in this directory:

    ./about
    ./help
    ./quick-start       <-- usage examples
    ./readme            <-- this file
    ./security-notes


---------------------------------------------------------------------------------------------------

Explorando algumas funcionalidades do IPFS:

 \\Usando o quick-start, que mostra comandos básicos de gerenciar e adcionar arquivos, 
configuração da Rede, do modo Online, criar pastas, entre outras funções. 

        ipfs cat /ipfs/QmYwAPJzv5CZsnA625s3Xf2nemtYgPpHdWEz79ojWnPbdG/quick-start   



----------------------------------------------------------------------------------------------------

Obs: Algo que deve ser Observado está relacionado a instalão do Pacote de atualização do IPFS,
em alguns casos, versões mais recentes, foram verificados alguns erros de configuração de  alocação de arquivos. Então a sugestão é usar versões como a 0.3.11 até 0.4.1.































