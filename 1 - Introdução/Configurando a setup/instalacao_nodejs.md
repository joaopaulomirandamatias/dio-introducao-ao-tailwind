## Instalação do NodeJS 

### Instalação no Windows

Para instalar o NodeJS no Windows, primeiro precisamos ir até a página oficial do [nodejs.dev](https://nodejs.dev/)

Depois, vamos clicar na versão LTS para baixar. A versão LTS é a mais estável, então a não ser que precisemos de alguma funcionalidade nova e mais atual do NodeJs, a versão LTS é a que devemos usar. Após baixar o instalador, basta executar e next > next...

Quando chegar na tela para selecionar as features, tenha a garantia de que pelo menos as opções `Node.js runtime`, `npm package manager` e `Add to PATH` estejam selecionadas.


Na próxima tela, o instalador vai perguntar se você gostaria de instalar outras ferramentas. Selecione a opção que vai instalar automaticamente essas ferramentas. É muito importante selecionar essa opção no Windows, porque alguns pacotes do npm não conseguem rodar nativamente no Windows sem algum tipo de compilação. Essas ferramentas vão cuidar da compatibilidade com o Windows.

Depois disso, é só concluir a instalação. Algumas janelas de terminal se abrirão automaticamente indicando o progresso da instalação.

>Após terminar a instalação, eu recomendo reiniciar a máquina, nem sempre é necessário, mas é uma garantia de que o NodeJS foi escrito corretamente no caminho do PATH do Windows.

Depois de todo esse processo, vamos rodar os seguintes comandos para garantir a instalação do NodeJS e do npm:

```	
node --version
npm --version
```	

### Instalação no Linux (Ubuntu)

A instalação no Linux é bem mais simples que no Windows. Vamos abrir o terminal e digitar o seguinte comando como super usuário:

```	
sudo apt-get install nodejs
```

 Após terminar o processo de instalação, podemos checar se o NodeJS e o npm foram instalados corretamente, usando os comandos:

 ```	
node --version
npm --version
```	