# Instalação do Linux

Sistemas operacionais baseados em Linux vêm sendo cada vez mais adotados em computadores domésticos e chegaram a registrar uma participação de 3,61% nos computadores do mundo, de acordo com dados da **NetMarketShare**.  

Pode parecer uma parcela pequena, mas corresponde a um recorde histórico dos sistemas operacionais do tipo e reflete uma trajetória de alta, já que o anterior era de 3,17%.

Os usuários que cogitam trocar de sistema operacional e adotar uma distribuição Linux podem acabar com dúvidas recorrentes, como quão seguro é o Linux, o que são termos como **Gnome** ou **KDE**, se há suporte para jogos ou qual o nível de oferta de apps para o sistema, por exemplo. 

Pensando nisso, nós aqui da **4Linux** preparamos um guia em detalhes, de como fazer para que você tenha um sistema Linux instalado. 

Instalar o Linux já foi uma tarefa bem desafiadora. Atualmente, é uma tarefa bem mais simples, mas requer atenção a alguns detalhes importantes, sobretudo em relação ao particionamento de disco. Não há um roteiro de instalação de Linux que sirva para todos os casos de uso, mas deve-se ficar atento às boas práticas como: 

* Isolar diretórios que tem gravação constante e que vários usuários utilizam, por exemplo, os diretórios **home** e **tmp**, para que não falte espaço em disco para o sistema operacional; 
* Isolar o diretório **home** facilita o backup e restauração do sistema operacional após uma formatação e aplicação de cotas de disco;
* Isolar o diretório **tmp** permite aplicar estratégias de segurança, como desabilitar execução de scripts maliciosos nesta pasta, uma vez que todo usuário pode executar scripts neste diretório;
* Isolar o diretório **/var/log** em uma partição para garantir que ele sempre terá um espaço mínimo para gravar registros de sistema e de aplicações;

## Introdução

O primeiro passo é baixar o arquivo ISO de instalação do sistema, para isso, faça o download do Debian **GNU/Linux 10 Buster** (lançado em 06 de julho de 2019) no seguinte site: http://cdimage.debian.org/debian-cd/

Estes são os Exemplos de configuração do **CentOS 8.x** que são compatíveis com o **Red Hat Enterprise Linux 8.x**. O **CentOS 8** foi lançado em 24 de setembro de 2019 e receberá suporte até maio de 2029. Faça o download do arquivo ISO do **CentOS 8.1** para instalação no site a seguir: https://mirrors.oit.uci.edu/centos/8.1.1911/isos/x86_64/ 

## Esquema de particionamento de disco

* **Tamanho do disco para máquina virtual**: 100 GB
* **Quantidade de partições**: 6

Obs.: Os valores aqui demonstrados se baseiam nas capacidades do computador utilizado para a criação da máquina virtual, e podem ser diferentes em outro ambiente de instalação.

&nbsp;

**Partição** | **Tamanho** | **Sistema de Arquivo** | **Ponto de Montagem**
:-----------:|:-----------:|:----------------------:|----------------------
/dev/sda1    |  50GB       |  ext4                  |       /
/dev/sda5    |  20GB       |  ext4                  |       /var
/dev/sda6    |  10GB       |  ext4                  |       /home
/dev/sda7    |  5GB        |  ext4                  |       /var/log
/dev/sda8    |  2,5GB      |  ext4                  |       /tmp
/dev/sda9    |  2,5GB      |  swap                  |


## Swap

Uma partição **swap** é usada para suportar a memória virtual. Em outras palavras, os dados são gravados numa partição **swap** quando não há memória RAM suficiente para armazenar os dados que seu sistema está processando.

Nos últimos anos, o tamanho recomendado para a partição swap cresceu conforme o aumento de memória RAM dos sistemas, e como esse aumento está na casa de centenas de gigabytes, hoje é entendido que a quantidade de espaço swap que um sistema precisa, deve ser determinada em função da carga de trabalho da memória executada naquele sistema. 

O espaço **swap** geralmente é designado durante a instalação, mas determinar a carga de trabalho desta memória em um sistema neste ponto pode ser difícil, por isso, você pode definir o tamanho de acordo com a tabela abaixo, conforme a quantidade de memória RAM que você possui.  

&nbsp;

Memória RAM do Sistema |	Tamanho mínimo de Espaço de Swap
:----------------:|:--------------------------------------:
4GB ou menos |	2GB 
4GB até 16GB  |	4GB 
16GB até 64GB  |	8GB 
64GB até 256GB  |	16GB 
256GB até 512GB |	32GB   


&nbsp;

### Instalação do Debian 10

![](imagens/Debian/001.png)

![](imagens/Debian/002.png)

![](imagens/Debian/003.png)

![](imagens/Debian/004.png)

![](imagens/Debian/005.png)

![](imagens/Debian/006.png)

![](imagens/Debian/007.png)

![](imagens/Debian/008.png)

![](imagens/Debian/009.png)

![](imagens/Debian/010.png)

![](imagens/Debian/011.png)

![](imagens/Debian/012.png)

![](imagens/Debian/013.png)

![](imagens/Debian/014.png)

![](imagens/Debian/015.png)

![](imagens/Debian/016.png)

![](imagens/Debian/017.png)

![](imagens/Debian/018.png)

![](imagens/Debian/019.png)

![](imagens/Debian/020.png)

![](imagens/Debian/021.png)

![](imagens/Debian/022.png)

![](imagens/Debian/023.png)

![](imagens/Debian/024.png)

![](imagens/Debian/025.png)

![](imagens/Debian/026.png)

![](imagens/Debian/027.png)

![](imagens/Debian/028.png)

![](imagens/Debian/029.png)

![](imagens/Debian/030.png)

![](imagens/Debian/031.png)

![](imagens/Debian/032.png)

![](imagens/Debian/033.png)

![](imagens/Debian/034.png)

![](imagens/Debian/035.png)

![](imagens/Debian/036.png)

![](imagens/Debian/037.png)

![](imagens/Debian/038.png)

![](imagens/Debian/039.png)

![](imagens/Debian/040.png)

![](imagens/Debian/041.png)

![](imagens/Debian/042.png)

![](imagens/Debian/043.png)

![](imagens/Debian/044.png)

![](imagens/Debian/045.png)

![](imagens/Debian/046.png)

![](imagens/Debian/047.png)

![](imagens/Debian/048.png)

![](imagens/Debian/049.png)

![](imagens/Debian/050.png)

![](imagens/Debian/051.png)

![](imagens/Debian/052.png)

![](imagens/Debian/053.png)

![](imagens/Debian/054.png)

![](imagens/Debian/055.png)

![](imagens/Debian/056.png)

![](imagens/Debian/057.png)

![](imagens/Debian/058.png)

![](imagens/Debian/059.png)

![](imagens/Debian/060.png)

![](imagens/Debian/061.png)

![](imagens/Debian/062.png)

![](imagens/Debian/063.png)

![](imagens/Debian/064.png)

![](imagens/Debian/065.png)

![](imagens/Debian/066.png)

![](imagens/Debian/067.png)

![](imagens/Debian/068.png)

![](imagens/Debian/069.png)

![](imagens/Debian/070.png)

![](imagens/Debian/071.png)

![](imagens/Debian/072.png)

![](imagens/Debian/073.png)

![](imagens/Debian/074.png)

![](imagens/Debian/075.png)

![](imagens/Debian/076.png)

![](imagens/Debian/077.png)

![](imagens/Debian/078.png)

![](imagens/Debian/079.png)

![](imagens/Debian/080.png)

![](imagens/Debian/081.png)

![](imagens/Debian/082.png)

![](imagens/Debian/083.png)

![](imagens/Debian/084.png)


#### Procedimentos comuns pós instalação

Se você acabou de instalar o Sistema Operacional, os passos a seguir podem ser efetuados, para melhor experiência de uso e comodidade.

* **Configurações iniciais:** Atualizar sistema

Mesmo que tenha instalado o sistema logo após seu lançamento, é interessante verificar se existem atualizações disponíveis.

Para isso no Debian temos o **APT**, a ferramenta que controla o que é instalado no seu sistema. 

O principal arquivo de configuração que o APT usa pra decidir de quais fontes ele deve baixar pacotes é `/etc/apt/sources.list`, mas ele também pode usar arquivos do diretório `/etc/apt/sources.list.d/` - para detalhes, veja: https://manpages.debian.org/buster/apt/sources.list.5.en.html 

Este é um exemplo do arquivo de repositórios do Debian:


```shell

deb http://deb.debian.org/debian buster main contrib non-free
deb-src http://deb.debian.org/debian buster main contrib non-free

deb http://deb.debian.org/debian-security/ buster/updates main contrib non-free
deb-src http://deb.debian.org/debian-security/ buster/updates main contrib non-free

deb http://deb.debian.org/debian buster-updates main contrib non-free
deb-src http://deb.debian.org/debian buster-updates main contrib non-free
```

```shell
root@localhost:~# apt update

Hit:1 http://deb.debian.org/debian buster InRelease
Get:2 http://deb.debian.org/debian buster-updates InRelease [46.8 kB]
Get:3 http://security.debian.org/debian-security buster/updates InRelease [39.1 kB]
Get:4 http://security.debian.org/debian-security buster/updates/main Sources [1,984 B]
Get:5 http://security.debian.org/debian-security buster/updates/main amd64 Packages [1,864 B]
Get:6 http://security.debian.org/debian-security buster/updates/main Translation-en [1,660 B]
Fetched 91.4 kB in 3s (33.2 kB/s)
Reading package lists... Done
Building dependency tree
Reading state information... Done
All packages are up to date.
```

```shell
root@localhost:~# apt upgrade  -y
```

* **Configurações iniciais:** Configurações do Vim

Toda distribuição Linux já vem com o `vi` instalado, entretanto o vim (vi improved) é hoje, sem dúvidas, o melhor editor de arquivos para quem trabalha diariamente com Linux. Sendo assim, eu sempre o instalo em servidores que costumo trabalhar. Para instalar o vim em distribuições baseadas no Debian basta rodar o comando abaixo com direitos de root.


* Instale o Vim:

```shell
[root@localhost ~]# apt install vim -y
```

Além disso também configuro o vim para que ele faça um destaque maior nos arquivos enquanto eu estiver editando. Para isso edite o arquivo vimrc que está dentro da pasta /etc/vim conforme os comandos abaixo.

```shell
 [root@localhost ~]# vi ~/.vimrc

set number                    " Numera as linhas
set linebreak                 " Quebra a linha sem quebrar a palavra
set nobackup                  " Não salva arquivos de backup~
set wildmode=longest,list     " Completa o comando com TAB igual o bash
set ignorecase                " Ignora o case sensitive nas buscas
set smartcase                 " Se tiver alguma letra maiúscula, ativa o case sensitive
set gdefault                  " Sempre substitui todas as palavras, não só a primeira
set smartindent               " Auto-indenta
set expandtab                 " Identa com espaços
set tabstop=2                 " Quantidade de espaços por indentação
set shiftwidth=2              " Quantidade de espaços da auto-indentação
set guioptions-=T             " Deixa a GUI sem a toolbar
set autochdir                 " Vai pro diretório do arquivo aberto
set cursorline                " Mostra linha atual mais clara
set hlsearch                  " Termo procurado em destaque
set pumheight=15              " Máximo de palavras no popup de autocomplete
set completeopt=menu,preview  " Como mostrar as possibilidade de inserção
set spelllang=pt              " Escolhe o dicionário
set foldenable                " Habilita agrupamento de blocos
set foldcolumn=1              " Exibie coluna com + e - para agrupamentos
set foldmethod=marker         " Define agrupamento por marcas
set foldmarker={,}            " Define marcas de agrupamento como { e }
set foldlevel=9999            " Inicia com todos os agrupamentos abertos
```

```shell
[root@localhost ~]# source ~/.bashrc 
```

### Instalação do CentOS 8

![](imagens/CentOS/001.png)

![](imagens/CentOS/002.png)

![](imagens/CentOS/003.png)

![](imagens/CentOS/004.png)

![](imagens/CentOS/005.png)

![](imagens/CentOS/006.png)

![](imagens/CentOS/007.png)

![](imagens/CentOS/008.png)

![](imagens/CentOS/009.png)

![](imagens/CentOS/010.png)

![](imagens/CentOS/011.png)

![](imagens/CentOS/012.png)

![](imagens/CentOS/013.png)

![](imagens/CentOS/014.png)

![](imagens/CentOS/015.png)

![](imagens/CentOS/016.png)

![](imagens/CentOS/017.png)

![](imagens/CentOS/018.png)

![](imagens/CentOS/019.png)

![](imagens/CentOS/020.png)

![](imagens/CentOS/021.png)

![](imagens/CentOS/022.png)

![](imagens/CentOS/023.png)

![](imagens/CentOS/024.png)

![](imagens/CentOS/025.png)

![](imagens/CentOS/026.png)

![](imagens/CentOS/027.png)

![](imagens/CentOS/028.png)

![](imagens/CentOS/029.png)

![](imagens/CentOS/030.png)

![](imagens/CentOS/031.png)

![](imagens/CentOS/032.png)

![](imagens/CentOS/033.png)

![](imagens/CentOS/034.png)

![](imagens/CentOS/035.png)

![](imagens/CentOS/036.png)

![](imagens/CentOS/037.png)

![](imagens/CentOS/038.png)

![](imagens/CentOS/039.png)

![](imagens/CentOS/040.png)

![](imagens/CentOS/041.png)

![](imagens/CentOS/042.png)

![](imagens/CentOS/043.png)

![](imagens/CentOS/044.png)

![](imagens/CentOS/045.png)

![](imagens/CentOS/046.png)

![](imagens/CentOS/047.png)

![](imagens/CentOS/048.png)

![](imagens/CentOS/049.png)

![](imagens/CentOS/050.png)

![](imagens/CentOS/051.png)

![](imagens/CentOS/052.png)

![](imagens/CentOS/053.png)

![](imagens/CentOS/054.png)

![](imagens/CentOS/055.png)

![](imagens/CentOS/056.png)

![](imagens/CentOS/057.png)

![](imagens/CentOS/058.png)


#### Procedimentos comuns pós instalação


* Configurações iniciais: Atualizar sistema

A ferramenta de gerenciamento de pacotes DNF (Dandified YUM) foi definida como padrão no RHEL 8 / CentOS 8.

No entanto, o comando [yum] também está localizado como um link para o [dnf], portanto, é possível usar [yum] ou [dnf] com o mesmo uso. Na verdade, os documentos oficiais no RedHat dão exemplos com o comando [yum] para o RHEL 8.
(os documentos neste site dão exemplos com o comando [dnf])

[yum] e [dnf] estão vinculados ao comando [dnf-3].


```shell
[root@localhost ~]# which yum

/usr/bin/yum
```

```shell
[root@localhost ~]# ll yum

ls: não foi possível acessar 'yum': Arquivo ou diretório inexistente
```

```shell
[root@localhost ~]# ll /usr/bin/yum

lrwxrwxrwx. 1 root root 5 dez 19 12:43 /usr/bin/yum -> dnf-3
```

```shell
[root@localhost ~]# rpm -q yum

yum-4.2.7-7.el8_1.noarch
```

```shell
[root@localhost ~]# clear
```

```shell
[root@localhost ~]# which yum

/usr/bin/yum
```

```shell
[root@localhost ~]# ll /usr/bin/yum

lrwxrwxrwx. 1 root root 5 dez 19 12:43 /usr/bin/yum -> dnf-3
```

```shell
[root@localhost ~]# which dnf

/usr/bin/dnf
```

```shell
[root@localhost ~]# ll /usr/bin/dnf

lrwxrwxrwx. 1 root root 5 dez 19 12:43 /usr/bin/dnf -> dnf-3
```

```shell
[root@localhost ~]# ll /usr/bin/dnf-3 

-rwxr-xr-x. 1 root root 1954 dez 19 12:43 /usr/bin/dnf-3
```

```shell
[root@localhost ~]# rpm -q yum

yum-4.2.7-7.el8_1.noarch
```

```shell
[root@localhost ~]# rpm -ql yum

/etc/dnf/protected.d/yum.conf
/etc/yum.conf
/etc/yum/pluginconf.d
/etc/yum/protected.d
/etc/yum/vars
/usr/bin/yum
/usr/share/man/man1/yum-aliases.1.gz
/usr/share/man/man5/yum.conf.5.gz
/usr/share/man/man8/yum-shell.8.gz
/usr/share/man/man8/yum.8.gz
```

```shell
[root@localhost ~]# ll /etc/yum.conf

lrwxrwxrwx. 1 root root 12 dez 19 12:43 /etc/yum.conf -> dnf/dnf.conf
```

```shell
[root@localhost ~]# ll /etc/yum/vars

lrwxrwxrwx. 1 root root 11 dez 19 12:43 /etc/yum/vars -> dnf/vars
```

Após a instalação, atualize o CentOS Server para o mais recente:

```shell
[root@localhost ~]# dnf -y upgrade 

CentOS-8 - AppStream                                      4.7 kB/s | 4.3 kB     00:00    
CentOS-8 - Base                                           4.4 kB/s | 3.9 kB     00:00    
CentOS-8 - Extras                                         546  B/s | 1.5 kB     00:02    
Dependências resolvidas.
Nada para fazer.
Concluído!
```

* Configurações iniciais: Configurações do Vim

Existem muitos casos para usar o editor de texto no terminal, por isso é mais conveniente instalar editor com recursos avançados como o Vim.

Instalar o Vim:

```shell
[root@localhost ~]# dnf -y install vim-enhanced 
```

Defina o **alias** de comando para o seu próprio ambiente:

```shell
[root@localhost ~]# vi ~/.bashrc

# add alias to the end

alias vi='vim'
# apply changes
```

Configure o Vim para o seu próprio ambiente. (configurações comuns para todos os usuários estão em [/etc/vimrc])

```shell
 [root@localhost ~]# vi ~/.vimrc

set number                    " Numera as linhas
set linebreak                 " Quebra a linha sem quebrar a palavra
set nobackup                  " Não salva arquivos de backup~
set wildmode=longest,list     " Completa o comando com TAB igual o bash
set ignorecase                " Ignora o case sensitive nas buscas
set smartcase                 " Se tiver alguma letra maiúscula, ativa o case sensitive
set gdefault                  " Sempre substitui todas as palavras, não só a primeira
set smartindent               " Auto-indenta
set expandtab                 " Identa com espaços
set tabstop=2                 " Quantidade de espaços por indentação
set shiftwidth=2              " Quantidade de espaços da auto-indentação
set guioptions-=T             " Deixa a GUI sem a toolbar
set autochdir                 " Vai pro diretório do arquivo aberto
set cursorline                " Mostra linha atual mais clara
set hlsearch                  " Termo procurado em destaque
set pumheight=15              " Máximo de palavras no popup de autocomplete
set completeopt=menu,preview  " Como mostrar as possibilidade de inserção
set spelllang=pt              " Escolhe o dicionário
set foldenable                " Habilita agrupamento de blocos
set foldcolumn=1              " Exibie coluna com + e - para agrupamentos
set foldmethod=marker         " Define agrupamento por marcas
set foldmarker={,}            " Define marcas de agrupamento como { e }
set foldlevel=9999            " Inicia com todos os agrupamentos abertos
```

```shell
[root@localhost ~]# source ~/.bashrc 
```

#### Segurança

Segurança é um fator fundamental para o gerenciamento de servidores, porém, muitas vezes, ele fica de lado, principalmente em projetos pequenos ou pessoais, onde por alguma particularidade seja necessário desabilitar o firewall do sistema. 
No caso de distribuições Linux, muitas delas já possuem fortes políticas de segurança. Distribuições como o CentOS e o RHEL, são caracterizadas como opções seguras dentro do Linux devido à proteção multinível do SELinux.

Entretanto, ter muitas medidas de segurança pode atrapalhar algumas tarefas rotineiras, e por isso, as vezes é necessário desabilitar algumas delas.

* **Firewall**

Um firewall faz o filtro de pacotes que passam na rede. Para configurar um firewall é necessário o conhecimento sobre a estrutura da rede em questão e dos diferentes protocolos envolvidos na comunicação, isto é, dos serviços que a rede usa para que eles não percam a comunicação.  O objetivo em ter uma máquina fazendo o papel de Firewall Gateway em nossa é rede é minimizar as tentativas de ataques que elas recebem, tentando impedir possíveis invasões e levantamento de informações.

É possível mostrar o status do serviço Firewall da seguinte maneira. (ativado por padrão)


```shell
[root@localhost ~]# systemctl status firewalld

*  firewalld.service - firewalld - dynamic firewall daemon
   Loaded: loaded (/usr/lib/systemd/system/firewalld.service; enabled; vendor p>
   Active: active (running) since Wed 2019-09-24 23:16:35 JST; 18min ago
     Docs: man:firewalld(1)
 Main PID: 801 (firewalld)
    Tasks: 2 (limit: 25025)
   Memory: 30.9M
   CGroup: /system.slice/firewalld.service
           └─801 /usr/libexec/platform-python -s /usr/sbin/firewalld --nofork ->

Sep 24 23:16:34 localhost.localdomain systemd[1]: Starting firewalld - dynamic >
Sep 24 23:16:35 localhost.localdomain systemd[1]: Started firewalld - dynamic f>

 # [Active: active (running) ***] means firewalld is running now
```

Se você não precisar do serviço Firewall devido algum motivo, por exemplo já possuir alguma máquina Firewall sendo executada na rede local, ou outro motivo, é possível parar e desativar o serviço Firewall no servidor CentOS, como segue.


stop service

```shell
[root@localhost ~]# systemctl stop firewalld
```

disable service

```shell
[root@localhost ~]# systemctl disable firewalld

Removed /etc/systemd/system/multi-user.target.wants/firewalld.service.
Removed /etc/systemd/system/dbus-org.fedoraproject.FirewallD1.service. 
```

* **SELinux**

O SELinux é uma ferramenta de segurança que restringe o acesso à módulos específicos do Kernel. Algumas distribuições Linux, como CentOS e RHEL, já trazem o firewall implementado por padrão como uma medida de segurança extra no sistema. Outras distribuições, como Debian, também permitem sua instalação.

O SELinux é gerenciado através de algumas regras chamadas “políticas”, que restringem ou permitem o uso de certas aplicações para partes essenciais do sistema. O problema é que criar essas políticas é muito difícil.

A ferramenta atualmente possui três modos:

* O modo Enforcing nega todos os acessos não autorizados. Neste modo, o SELinux é considerado como habilitado.
* No modo Permissive, diferente do modo anterior, é permitido o acesso não autorizado, mas com a exibição de avisos.
* Em modo Disable o SELinux está desabilitado e permite todos os acessos sem avisos.


É possível desabilitar o SELinux temporariamente ou permanentemente, cada um com seus benefícios. Desabilitar temporariamente permite realizar testes sem precisar sacrificar a segurança do sistema. Assim que o sistema é reiniciado, o SELinux é ativado novamente.

Por outro lado, desativar o firewall permanentemente torna possível trabalhar mais rápido, principalmente em projetos pequenos ou médios. É importante lembrar que atualmente as distribuições do Linux possuem ótimas políticas de segurança, então desativar o SELinux não é tão prejudicial.

É possível mostrar o status atual do SELinux (Security-Enhanced Linux) da seguinte maneira. (ativado por padrão)


```shell
[root@localhost ~]# getenforce
Enforcing     # SELinux is enabled
```

Se você ativar o SELinux, pode haver casos de precisar modificar suas políticas manualmente, porque algumas vezes o ele interrompe os aplicativos. 

Se você não precisar do uso do SELinux, por ter o servidor executando apenas na Rede de segurança local, ou qualquer outro motivo, é possível desativar esse recurso da seguinte forma.


```shell
 [root@localhost ~]# vim /etc/selinux/config

 # This file controls the state of SELinux on the system.
 # SELINUX= can take one of these three values:
 #     enforcing - SELinux security policy is enforced.
 #     permissive - SELinux prints warnings instead of enforcing.
 #     disabled - No SELinux policy is loaded.
 # change the value below
 # enforcing  ⇒ enabled
 # disabled   ⇒ disabled
 # permissive ⇒ enabled but only loging, not deny accesses
 SELINUX=disabled
 # SELINUXTYPE= can take one of these two values:
 #     targeted - Targeted processes are protected,
 #     minimum - Modification of targeted policy. Only selected processes are protected.
 #     mls - Multi Level Security protection.
 SELINUXTYPE=targeted

 # restart computer to apply setting

[root@localhost ~]# reboot
```




