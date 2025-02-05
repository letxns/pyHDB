---
title: Documentação
author: Eric Brasil
date: 2022-08-26
---
# Bem-vindo à documentação da pyHDB - Ferramenta heurística para a Hemeroteca Digital Brasileira

<img src="img/banner.png" alt="Banner da pyHDB">

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![DOI](https://zenodo.org/badge/413270192.svg)](https://zenodo.org/badge/latestdoi/413270192)

[**Acesse o site de documentação da pyHDB aqui**](https://ericbrasiln.github.io/pyHDB/)

Ferramenta de auxílio metodológico para pesquisa na [Hemeroteca Digital Brasileira](memoria.bn.br/hdb) da Biblioteca Nacional.

Desenvolvida por [Eric Brasil](https://ericbrasiln.github.io) como parte de pesquisa acadêmica da área de História Digital.

>Essa ferramenta não possui fins lucrativos nem pretende acessar dados sigilosos ou alterar informações nos servidores da instituição.

Tem como objetivo auxiliar pesquisadores e pesquisadoras no processo de documentação e registro preciso das etapas de pesquisa e garantir o rigor metodológico. Portanto, é uma ferramenta heurística digital.

Seu desenvolvimento está no âmbito das pesquisas realizadas no curso de História do IHLM/Unilab e do [LABHDUFBA](http://www.labhd.ufba.br).

Os resultados da pesquisa serão publicados em artigo científico avaliado por pares na [Revista História da Historiografia](https://www.historiadahistoriografia.com.br/) em 2022 e seu código e documentação serão disponibilizados publicamente, com [licença MIT](LICENSE).

Buscamos não sobrecarregar os servidores da Biblioteca Nacional e respeitar os termos de uso. 

## Instalação

### Python
Essa ferramenta foi escrita em [Python 3.9](https://www.python.org/). Esta é uma linguagem de programação que te permite trabalhar rapidamente e integrar diferentes sistemas com maior eficiência.

Para executar o arquivo `.py` é preciso instalar o Python3 em seu computador, assim como as bibliotecas utilizadas na ferramentas.

[Clique aqui](https://python.org.br/instalacao-windows/) para um tutorial de instalação do Python no Windows, [clique aqui](https://python.org.br/instalacao-linux/) para Linux e [clique aqui](https://python.org.br/instalacao-mac/)
para Mac.

Após a instalação, vc pode executar arquivos `.py` direto do prompt de comando do Windows ou pelo terminal do Linux, ou utilizar as diversas [IDE](https://pt.wikipedia.org/wiki/Ambiente_de_desenvolvimento_integrado) disponíveis. 

Para saber mais sobre a instalação e configuração do Python em vários sistemas operacionais, veja a lição [Introdução e instalação do Python](https://programminghistorian.org/pt/licoes/introducao-instalacao-python) de William J. Turkel e Adam Crymble [^1].

Além do Python, seu computador precisa ter o pip instalado, um programa para instalar pacotes de software. Nas versões mais recentes do Python, o pip já vem instalado. Para saber mais, veja a lição [Instalação de Módulos Python com pip](https://programminghistorian.org/pt/licoes/instalacao-modulos-python-pip), de Fred Gibbs [^2].

[^1]: William J. Turkel e Adam Crymble, "Introdução e instalação do Python", traduzido por Josir C. Gomes, Programming Historian em português 1 (2021), [https://doi.org/10.46430/phpt0004](https://doi.org/10.46430/phpt0004).

[^2]: Fred Gibbs, "Instalação de Módulos Python com pip", traduzido por Felipe Lamarca, Programming Historian em português 1 (2021), [https://doi.org/10.46430/phpt0018](https://doi.org/10.46430/phpt0018).

#### Bibliotecas e módulos

- **urllib.requests**: módulo do Python que lida com urls.
[Saiba mais.](https://docs.python.org/pt-br/3/library/urllib.request.htmll)
- **Selenium**: o [Selenium](https://www.selenium.dev/documentation/en/) é um conjunto de ferramentas para automatização de utilização de navegadores.
- **webdriver.manager**: biblioteca que auxilia na instalação e configuração dos drivers de navegadores. [Saiba mais](https://pypi.org/project/webdriver-manager/)
- **pandas**: [Pandas](https://pandas.pydata.org/) é uma biblioteca escrita em Python para manipulação e análise de dados.
- **wget**: [Wget](https://www.gnu.org/software/wget/) é um programa de linha de comando para baixar arquivos de um servidor remoto.

>**OBS 1**: A ferramenta foi desenvolvida e testada no sistema operacional Linux, em distribuição baseada no Ubuntu 20.10. Entretanto, ela foi projetada para funcionar em qualquer sistema operacional que suporte o Python 3.9. 

> **OBS 2**: A ferramenta utiliza padrões ANSI para imprimir na tela alguns textos coloridos. Esse padrão é suportado nos terminais Linux e neles foram testados. Para usuários Windows é importante destacar que o suporte às *ANSI scape colors* existe no *PowerShell* a partir da versão 7.2, conforme essa [resposta no StackOverflow](https://stackoverflow.com/questions/70853849/powershell-formatting-issue-arm-template-whatif-ansi-escape-color/70855231#70855231). Portanto, para que os detalhes coloridos da ferramenta sejam impressos corretamente na tela, usuários de Windows devem utilizar PowerShell 7.2 ou mais recentes ou outros emuladores de terminal que suportem cores ANSI. Para mais informações ver a [página oficial do PowerShell](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_ansi_terminals?view=powershell-7.2) e a [página da Wikipédia sobre xterm](https://en.wikipedia.org/wiki/Xterm), emulador de terminal para Windows.

>**OBS 3**: É necessário possuir o navegador *Chrome* instalado, pois este será utilizado pelo Selenium para acessar o site da HDB.

### Download da ferramenta `pyHDB` 

Para baixar a ferramenta para seu computador, existem duas formas. Para ambos os casos, é necessário acessar o repositório do GitHub [ericbrasiln/pyHDB](https://github.com/ericbrasiln/pyHDB/) e clicar no botão `Code`.

![Botão](img/gh_1.png)

#### Baixar o arquivo compactado `pyHDB.zip`

Para baixar o arquivo `pyHDB.zip`, após clicar em `Code`, clique em `Download ZIP` e salve em seu computador.

![Download ZIP](pyHDB-docs/docs/img/gh_2.png)

Em seguida, descompacte o arquivo no local de sua preferência.

#### Clonar o repositório com Git ou criar um fork no GitHub

Para quem utiliza o sistema de controle de versões Git, basta clonar o repositório para seu computador, executando os comandos a partir da pasta em que deseja salvar o repositório.

```{.sh .bash}
git clone https://github.com/ericbrasiln/pyHDB.git
```

Quem utiliza o GitHub, pode também criar um *fork* do repositório.

### Instalando requisitos

Após baixar ou clonar o repositório para seu computador, acesse a pasta através do terminal ou PowerShell, caso seja usuário Windows.

```{.sh .bash}
cd <caminho para pasta>/pyHDB/src
```

Para saber mais sobre os comandos básicos do PowerShell, veja a lição [Introduction to the Windows Command Line with PowerShell](https://programminghistorian.org/en/lessons/intro-to-powershell), de Ted Dawson no The Programming Historian [^3]. Para o Terminal para Linux e MacOS, veja a lição [Introduction to the Bash Command Line](https://programminghistorian.org/en/lessons/intro-to-bash), de Ian Milligan and James Baker no The Programming Historian [^4].

[^3]: Ted Dawson, "Introduction to the Windows Command Line with PowerShell," Programming Historian 5 (2016), https://doi.org/10.46430/phen0054.

[^4]: Ian Milligan and James Baker, "Introduction to the Bash Command Line," Programming Historian 3 (2014), https://doi.org/10.46430/phen0037.

É necessário instalar os requisitos ([módulos e bibliotecas](#bibliotecas-e-modulos)). Para isso, execute o comando abaixo:

```{.sh .bash}
$ pip3 install -r requirements.txt
```
Após a conclusão do processo, a ferramenta estará pronta para ser utilizada.

## Usos

Para iniciar a ferramenta, é preciso executar o arquivo `pyHDB.py` usando Python3, a partir da pasta `pyHDB/src`. Para isso, execute o comando abaixo, no terminal ou PowerShell, estando na pasta `pyHDB/src`.

```{.sh .bash}
$ python3 pyHDB.py
```

Ao executar o programa, o usuário verá as informações introdutórias da ferramentas, como na imagem abaixo:

<img src="pyHDB-docs/docs/img/intro.png" alt="intro pyHDB">

Em seguida, o usuário deverá inserir os parâmetros de busca. Lembrando que nessa versão do programa, a busca inicial é estabelecida pela opção `local`. 

``` 
1- Local
Orientações para busca:
      - O termo deve ser idêntico às opções listadas na página da HDB;
      - Esse parâmetro é case sensitive;
Digite o local de busca: 
``` 
É possível incluir uma opção de recorte temporal em seguida. 

```

2 - Período
Orientações para busca:
      - O recorte deve ser escrito de forma idêntica às opções listadas na página da HDB;
      - É possível buscar todos os periódicos digitando `Todos`
Digite o período de busca: 
``` 

>**OBS 4**: Lembrando que os parâmetros `Local` e `Período` devem ser escritos de forma idêntica às opções listadas na [página da HDB](http://memoria.bn.br/hdb/). Por Exemplo, se o usuários deseja buscar os periódicos existentes no Rio de Janeiro, deve colocar `RJ`. Se o usuário deseja buscar os periódicos existentes no Rio de Janeiro na década de 1910, deve colocar `1910 - 1919`, pois as opções de período existentes na HDB estão organizadas por décadas.

A busca será efetuada em todos os acervos existentes para essa configuração (`3 - Periódico: Todos`), após a inclusão do termo da busca.

```
4 - Termo da busca
Orientações para busca:
      - Coloque o termo entre aspas duplas para expressões exatas;
      - Não use acentos ou caracteres especiais;
      - É recomendado não utilizar mais do que três palavras.
Digite o termo de busca:
```

Portanto, a busca foi elaborada a partir das demandas de pesquisa e interesses pessoais e serão explicadas detalhadamente em artigo. 

A partir dos parâmetros de busca definidos pelo usuário, o programa retorna todos os acervos dos jornais com alguma ocorrência, até o limite de 100 jornais (ou seja, a segunda página de resultados).

### Opção de busca por acervo ou lista de acervos específicos

A ferramenta `pyHDB` permite a busca por acervos específicos, ou lista de acervos específicos. Para tanto é preciso executar o arquivo `pyHDB_acervos.py`.

O usuário deverá informar o número do acervo ou a lista de acervos que deseja pesquisar.

Essa opção foi desenvolvida para sanar erros no processo de raspagem que podem acontecer principalmente em buscas com milhares de ocorrências. 

Se algum acervo não for raspado corretamente pela ferramenta principal `pyHDB`, o usuário poderá executar o arquivo `pyHDB_acervos.py` para raspagem de acervos específicos.

Ao final do processo, a ferramenta criará arquivos `csv` e relatórios em `txt` no mesmo padrão da ferramenta principal `pyHDB`. Além disso, retornará automaticamente um `csv` final mesclando os dados recém coletados com os dados já existentes (desde que a busca seja executada na mesma data).

## Resultados

O programa retorna os seguintes resultados:

1. Cria diretórios de armazenamento: `HDB/{termo da busca}/{data da busca}/`

2. `CSV`: Cria um diretório `HDB/{termo da busca}/{data da busca}/CSV` e, dentro dele, salva arquivo csv contendo os seguintes dados para cada ocorrência: `Termo da busca, Data da Busca, Acervo, Ano, Edição, Página, Nome do arquivo, Link`.

3. `RELATÓRIOS`: Cria um diretório `HDB/{termo da busca}/{data da busca}/RELATÓRIOS` e salva nele relatórios de busca para cada pesquisa.
   - GERAL: Com os dados gerais da pesquisa
        ``` 
        - Data e hora da busca
        - Local da busca
        - Período da busca
        - Periódico da busca: 
        - Termo da busca
        - Lista de acervos com ocorrências (máx. de 100) e quantidade de ocorrências
        - Total de acervos com ocorrências (máx. de 100)
        - Informações adicionais: Total de páginas pesquisadas; Total de acervos pesquisados; Total de ocorrências e Frequência de ocorrências por página.
        ```
        O título do arquivo tem o seguinte padrão: `GERAL_{termo da pesquisa}_{data e hora da busca}.txt`
   - Acervo: Com os dados de cada acervo
        ``` 
        - Data e hora da busca
        - Termo da busca
        - Acervo
        - Total de ocorrências
        - Link da lista de resultados
        ```
        O título do arquivo tem o seguinte padrão: `relatório_{nome do acervo}_{número do acervo}_{data e hora da busca}.txt`
   - ERRO: registra acervos que não puderam ser raspados
        ``` 
        - Data e hora da busca
        - Termo da busca
        - Acervo com ocorrência que não pode ser acessado
        ```
        O título do arquivo tem o seguinte padrão: `ERRO_{número do acervo}_{data e hora da busca}.txt`
   - INFORMAÇÕES GERAIS: registra dados gerais relativo ao quantitativo de acervos e páginas pesquisadas na busca e a quantidade de ocorrências, assim como a frequência de ocorrências por página.
        - Acervo
        - Total de Páginas
        - Total de Ocorrências
        - Frequência de ocorrências X páginas. 
        O título do arquivo tem o seguinte padrão: `{infos_acervos}_{período}_{page01 ou 02}.csv`
4. `ARQUIVOS_IMG`: Cria um diretório `HDB/{termo da busca}/{data da busca}/ARQUIVOS_IMG`e salva as imagens das páginas com ocorrências. O nome do arquivo é a combinação no número do acervo com o número geral da página. Ex: `168319_02_12603.jpg`

### Estrutura de diretórios

```
HDB
├── {termo da busca}
│   ├── {data}
│   │   ├── CSV
│   │   ├── RELATÓRIOS
│   │   ├── ARQUIVOS_IMG
```

## Relatar erros e sugestões

Sendo a ferramenta `pyHDB` um scraper, um raspador de dados da internet, ela está profundamente ligada e dependente da estrutura e funcionamento do site da Hemeroteca Digital Brasileira da Biblioteca Nacional. Instabilidades no funcionamento do site da HDB afetam e prejudicam a raspagem de dados. Assim como, alterações na estrutura do site da HDB podem inviabilizar o funcionamento da ferramenta.

Portanto, erros de execução, de resultados, entre outros podem acontecer a qualquer momento. Para que a ferramenta possa continuar funcionando corretamente, o usuário deverá relatar os erros e enviar sugestões para a equipe de desenvolvimento da ferramenta.

Sugerimos que o usuário crie [`issues` no GitHub da ferramenta `pyHDB`](https://github.com/ericbrasiln/pyHDB/issues) explicando da forma mais detalhada possível os problemas e qual sistema operacional está utilizando. 

## Como citar?

É possível clicar em `Cite this repository` na aba à direita da página inicial do repositório no GitHub para acessar a citação nos formatos APA e BibTex, ou ainda acessar o [arquivo da citação](CITATION.cff) em formato .cff.

Abaixo a citação no formato BibTex:

```
@software{Eric_pyhdb2021,
  author = {Eric Brasil},
  doi = {10.5281/zenodo.5696671}
  title = {pyHDB - Ferramenta heurística para a Hemeroteca Digital Brasileira},
  url = {https://github.com/ericbrasiln/pyHDB}
  version = {1.4}
  year = {2021},
  note = {Online; accessed 08 April 2022}
}
```

***

## Agradecimentos

Agradeço ao LABHDUFBA pela parceria e possibilidades de aprendizado e desenvolvimento de ferramentas e reflexões para a pesquisa em história e humanidades digitais.

A **pyHDB** não seria possível sem a participação ativa de Leonardo F. Nascimento (a quem devo o agradecimento pela sugestão do nome da ferramenta) e Gabriel Andrade.

***

## Licença

[MIT LICENSE](LICENSE)

Copyright (c) 2021 [Eric Brasil](https://ericbrasiln.github.io/)
