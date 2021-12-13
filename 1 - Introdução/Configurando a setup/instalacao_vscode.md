## Instalação do Visual Studio Code

### Instalação no Windows

A instalação no Windows é relativamente simples, basta acessar o site oficial do  [Visual Studio Code](https://code.visualstudio.com/) e fazer o Download da sua última versão, clicando no botão "Download for Windows".

Em seguida, execute o instalador baixado e siga as instruções na tela, não esqueça de marcar a opção `Add to Path` para adicionar o Visual Studio Code nas variáveis de ambiente.

Finalizada a instalação, feche todos os terminais abertos e abra um novo e digite o comando abaixo.

```
code --version
```

Se tudo ocorrer como esperado, você verá a versão do Visual Studio Code instalada em sua máquina e estará tudo pronto para prosseguir.

### Instalação no Linux (Ubuntu)

A instalação no Linux é relativamente simples, basta acessar o site oficial do [Visual Studio Code](https://code.visualstudio.com/) e fazer o Download da sua última versão, clicando no botão "Download for Linux".

Como resultado do Download você terá um pacote `.deb` na pasta Downloads. Abra um terminal, navegue até a mesma e execute o seguinte comando.

```	
sudo apt install ./NOME_ARQUIVO_BAIXADO.deb
```
Pronto, a instalação do Visual Studio Code está realizada e ele já deve aparecer no menu de aplicativos para você.

### Adicionando ao PATH

Podemos ainda adicionar o Visual Studio Code ao `PATH` para ter acesso ao comando code no terminal, podendo abrir diretamente pastas de lá no Visual Studio Code.

Abra seu menu de aplicativos e inicie o Visual Studio Code e na tela inicial dele pressione F1 para abrir a tela de execução de comandos.

Procure pelo comando `Shell Command: Install 'code' command in PATH` para adicionar o Visual Studio Code ao PATH do seu sistema operacional.