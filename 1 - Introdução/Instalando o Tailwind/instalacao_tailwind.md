## Instalação do Tailwind CSS

A utilização do Tailwind CSS é uma boa prática para o desenvolvimento de sites modernos.

O Tailwind CSS funciona verificando todos os seus arquivos HTML, componentes JavaScript e quaisquer outros modelos em busca de nomes de classes, gerando os estilos correspondentes e gravando-os em um arquivo CSS estático.

É rápido, flexível e confiável - com tempo de execução zero.

Nessa aula iremos aprender como instalar o Tailwind CSS e como utilizá-lo no projeto.

1. Instalação do Tailwind CSS utilizando CDN

> CDN é abreviação de Content Delivery Network (ou Rede de Distribuição de Conteúdo). É uma rede de servidores (pontos de presença) que armazenam réplicas do conteúdo de outros sites na memória (cache) e depois os entrega aos visitantes, baseando-se na localização geográfica para conectá-los ao servidor mais próximo e mais rápido, reduzindo o tempo de transferência dos dados (latência).

Use o Play CDN para experimentar o Tailwind diretamente no navegador, sem qualquer etapa de construção. O Play CDN foi projetado apenas para fins de desenvolvimento e não é a melhor escolha para produção.

### Adicione o script Play CDN ao seu HTML

````
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
````
Para teste pode utilizar o [Play CDN](https://play.tailwindcss.com/) o playground oficial do Tailwind CSS.


2. Instalação do Tailwind CSS utilizando o CLI

A maneira mais simples e rápida de começar a usar o Tailwind CSS do zero é com a ferramenta Tailwind CLI.

Mas antes temos que iniciar um projeto usando o nodejs. O comando `$ npm init` nos permite iniciar um pacote, criando o arquivo `package.json` de acordo com certas respostas que damos às perguntas feitas.

Mas você pode pular as perguntas, fazendo com que o arquivo `package.json` seja criado imediatamente. Basta adicionar `-y` ao comando: `$ npm init -y`.

```
npm init -y
```

Instale __tailwindcss__ via npm e crie seu tailwind __config.js__ arquivo.

```
npm install -D tailwindcss
npx tailwindcss init
```

### Configure seus caminhos de modelo
Adicione os caminhos para todos os seus arquivos de modelo em seu __tailwind.config.js__ arquivo.

```	
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### Adicione as diretivas do Tailwind ao seu CSS
Adicione as __@tailwind__ diretivas para cada uma das camadas do Tailwind ao seu arquivo CSS principal.

```	
@tailwind base;
@tailwind components;
@tailwind utilities;
```	

### Inicie o processo de compilação da CLI do Tailwind
Execute a ferramenta CLI para examinar seus arquivos de modelo em busca de classes e construir seu CSS.

```	
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```	

### Comece a usar o Tailwind em seu HTML
Adicione seu arquivo CSS compilado ao `<head>` e comece a usar as classes de utilitários do Tailwind para estilizar seu conteúdo.

```	
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/dist/output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```

