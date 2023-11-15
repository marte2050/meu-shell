# Meu Sell :zap:

## 1. Melhorando a produtividade

<p align="justify">
  Quando estamos desenvolvendo aplicações é essencial que tenhamos um shell que atenda as nossas necessidades e seja fácil de personalizar. No ambiente Linux temos diversas opções como bash, sh, zsh e entre outros, ao qual cada um com seus prós e contras. 
  
  Atualmente, o Zsh tem se destacado no mundo Linux em virtude de uma gama extensa de plugins e temas, ao qual possibilita aos usuários personalizá-lo de acordo com suas necessidades.
 </p>

<hr/>

### 1.2 Processo de instalação

<p> Para instalar o Zsh no Ubuntu podemos utilizar o comando abaixo: </p>

```bash
sudo apt update
sudo apt-get install zsh curl git
```

<hr/>

### 1.3 Oh My Zsh

<p align="justify">  Oh My Zsh é uma gerenciador para Zsh, ao qual provê milhares de funções úteis, plugins, temas e algumas outras coisitas mais... Para instalar o oh my zsh basta executar o comando abaixo. </p>

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

<hr/>

### 1.4 Instalando plugins para o Zsh

#### 1.4.1. zsh-syntax-highlighting

<p align="justify">  É um verificador de sintaxe em tempo de digitalização, ou seja, enquanto você digita é feito a verificação da sintaxe. Caso a digitalização esteja correta o texto ficará verde, caso contrário ficará vermelho. Para instalar utilize o comando abaixo: </p>

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
<hr/>

#### 1.4.1. zsh-autosuggestions

<p align="justify">  Zsh-autosuggestions faz o processo de sugestão de comandos com base nos históricos do terminal. </p>

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
<hr/>

### 1.5 Instalando temas para o Zsh

#### 1.5.1 Instalando Spaceship

<p align="justify">  Spaceship é um tema extremamente customizável que nos permite adicionar diversos recursos úteis para o dia-dia de um programador. </p>

Para instalar execute o comando abaixo:

```bash
git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1

ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"
```
<hr/>

#### 1.5.2 Definindo parâmetros para o nosso terminal spaceship


```

~/.zshrc
SPACESHIP_PROMPT_ORDER=(
    python
    git
    exec_time
    line_sep
    char
)

SPACESHIP_PROMPT_ADD_NEWLINE=true
SPACESHIP_CHAR_SYMBOL="❯"
SPACESHIP_CHAR_SUFFIX=" "

```
