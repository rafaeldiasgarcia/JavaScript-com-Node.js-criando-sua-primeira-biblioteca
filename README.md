# Node.js Library - Aula 5

Este projeto é uma biblioteca Node.js desenvolvida durante a aula 5 do curso de JavaScript com Node.js da Alura. A biblioteca processa arquivos de texto para identificar palavras duplicadas em cada parágrafo.

## Estrutura do Projeto

```
README.md
3709-nodejs-lib-aula-5/
    3709-nodejs-lib-aula-5/
        .gitignore
        package.json
        arquivos/
            texto-aprendizado.txt
            texto-kanban.txt
            texto-web.txt
        resultados/
            resultado.txt
        src/
            cli.js
            helpers.js
            index.js
            erros/
                funcoesErro.js
```

## Instalação

1. Clone o repositório:
    ```sh
    git clone <URL_DO_REPOSITORIO>
    ```
2. Navegue até o diretório do projeto:
    ```sh
    cd 3709-nodejs-lib-aula-5/3709-nodejs-lib-aula-5
    ```
3. Instale as dependências:
    ```sh
    npm install
    ```

## Uso

Para processar um arquivo de texto e identificar palavras duplicadas, execute o seguinte comando:

```sh
node src/cli.js -t <caminho_do_texto> -d <caminho_do_destino>
```

- `<caminho_do_texto>`: Caminho para o arquivo de texto a ser processado.
- `<caminho_do_destino>`: Caminho para a pasta onde o arquivo de resultados será salvo.

Exemplo:

```sh
node src/cli.js -t arquivos/texto-aprendizado.txt -d resultados
```

## Estrutura do Código

- `src/cli.js`: Arquivo principal que lida com a linha de comando e chama as funções necessárias para processar o arquivo de texto.
- `src/helpers.js`: Contém funções auxiliares para filtrar ocorrências e montar a saída do arquivo.
- `src/index.js`: Contém as funções principais para contar palavras e verificar palavras duplicadas.
- `src/erros/funcoesErro.js`: Contém a função para tratar erros.

## Dependências

- `chalk`: Biblioteca para estilizar a saída do terminal.
- `commander`: Biblioteca para criar interfaces de linha de comando.

## Licença

Este projeto está licenciado sob a licença ISC.