# Oh My Zsh

# Importante: <font color="red">Nunca instale no servidor</font>, sempre no seu micro local

## 1) Pré requisitos 
(Obs: para instalar entre no terminal e digite sudo su)
### 1.1) Ter o zsh instalado
### Debian / Ubuntu / ...
```
apt-get install zsh
```
### RedHat / CentOS / ...
```
yum -y install zsh
```
### 1.2) Ter o curl ou wget instalado
### Debian / Ubuntu / ...
```
O Debian já vem com o wget instalado
```
### RedHat / CentOS / ...
```
O CentOS já vem com o curl instalado
```
### 1.3) Ter o git instalado
### Debian / Ubuntu / ...
```
apt-get install git git-doc
```
### RedHat / CentOS / ...
```
yum -y install git
```
## 2) Instalando o Oh My Zsh <a href="https://ohmyz.sh/">Site Oficial</a>
### Pode ser istalado usando o curl ou o wget
### Usando o curl
```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
### Usando o wget
```
sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```
## 3) Aceite a mudança do seu shell padrão para o zsh digitando Y ou y se for apresentada a pergunta abaixo
```
Do you want to change your default shell to zsh? [Y/n]
```
## 4) Instalando o tema agnoster <a href="https://github.com/agnoster/agnoster-zsh-theme">Repositório Oficial</a>
Clone o repositório com o comando:
```
git clone https://github.com/agnoster/agnoster-zsh-theme.git
```
Será criada/o uma pasta/diretório chamada agnoster-zsh-theme
Entre na pasta .oh-my-zsh usando o comando:
```
cd .oh-my-zsh
```
Entre na pasta themes usando o comando:
```
cd themes
```
Copie o arquivo agnoster-zsh-theme que foi criado na pasta agnoster-zsh-theme usando o comando:
```
cp ../../agnoster-zsh-theme/agnoster.zsh-theme .
```
## 5) Para que o tema venha a funcionar corretamente instale a fonte Poweline-patched <a href="https://github.com/powerline/fonts">Repositório Oficial</a>
Volte a sua home usando o comando:
```
cd ~
```
### Debian / Ubuntu / ...
```
apt-get install fonts-powerline
```
### RedHat / CentOS / ...
```
git clone https://github.com/powerline/fonts.git --depth=1
cd fonts
./install.sh
cd ..
rm -rf fonts
```
### 6) Habilite o tema agnoster
### Faça um backup do arquivo de configuração com o comando:
```
cp .zshrc zshrc-bkp
```
### Clone este repositório com o comando:
```
git clone https://github.com/paulo-correia/Oh_My_Zsh__Help.git

```
Execute o script com os comandos:
```
cd Oh_My_Zsh__Help
./muda_tema.sh

```
### 7) Feche o terminal e entre novamente
Já estará istalado o Oh My Zsh com o tema agnoster

Caso aprenente o erro "oh-my-zsh/themes/agnoster.zsh-theme:27: unknown file attribute"
### Faça um backup do tema de configuração com os comando:
```
cd .oh-my-zsh/themes
cp agnoster.zsh-theme agnoster-bkp
```
Copie o tema modificado em cima do original com o comando:
```
cd ../../
cp Oh_My_Zsh__Help/agnoster.zsh-theme .oh-my-zsh/themes
```

