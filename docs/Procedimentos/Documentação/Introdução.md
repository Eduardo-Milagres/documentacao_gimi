# Introdução
## Objetivo
- Facilitar a troca de informação entre os setores;
- Padronização;
- Correção de erros;
- Aprendizado contínuo.

## Pré requisitos para elaboração da documentação
- Conhecimento básico em [markdown](#markdown)
- Instalação do [python]({{ links.python }})
- Instalação do [MKDocs](#mkdocs)

## Markdown
Os arquivos da documentação são escritos em [markdown]({{ links.markdown }}).
Markdown é uma linguagem de marcação que utiliza simbolos para formação, os principais simbolos podem ser consultados no [cheat sheet](https://www.markdownguide.org/cheat-sheet/).

## MKDocs
Essa documentação é escrita com [markdown]({{ links.markdown }}) e gerada pelo [MKDocs]({{ links.mkdocs }}), uma ferramenta de feração de sites estáticos.

O [MKDocs]({{ links.mkdocs }}) transforma os arquivos escritos em [Markdown](#Markdown) em páginas web.

Para melhor apresentação da documentação o tema escolhido foi o [Material](#Material).

### Pré requisitos
Para utilização do [MKDocs]({{ links.mkdocs }}) é necessário ter o [python]({{ links.python }}) e o gerenciador de pacotes pip instalados.
O [python]({{ links.python }}) pode ser baixado na página de [downloads]({{ links.python_download }}).

{{ imagens.python_instalacao }}

### Instalação do MKDocs
No terminal / cmd digite:

```bash
pip install mkdocs
```

Para instruções mais detalhadas e solução de dúvidas, vá ao site de [instalação do MKDocs]({{ links.mkdocs_instalacao }})

### Utilização do MKDocs
#### Criação da documentação
Para rodar o {{ links.mkdocs }}, no terminal / cmd rode o comando:

```bush
mkdocs new nome_da_pasta_de_documentação
```

Para esse projeto foi utilizada a pasta padrão do {{ links.mkdocs }}.

```bush
mkdocs new .
```

Após rodar o comando, o {{ links.mkdocs }} irá criar uma pasta .docs, onde serão armazenadas todos os arquivos da documentação.

#### Vizualização da documentação
Para vizualizar a documentação criada, rode o comando:

```bush
mkdocs serve
```

O comando irá rodar um servidor local (na máquina do usuário) onde a documentação pode ser vizualizada.

#### Gerar a documentação
Para que a documentação seja acessível para todos os usuários ela deve ser independete, ou seja, os usuários que irão vizualizar a documentação não devem se preocupar com os [pré requisitos](#pré-requisitos).
Para isso, após o término da documentação rode o comando:

```bush
mkdocs build
```

O comando transformará todos os arquivos {{ links.markdown }} em arquivos html que podem ser acessados por todos os navegadores, esses arquivos serão criados na pasta *site*.

## Material
O [material]({{ links.material }}) é um tema aplicado ao [MKDocs]({{ links.mkdocs }}) para alterar o layout das páginas e adicionar algumas funcionalidades. O [material]({{ links.material }}) é o tema mais utilizado nas documentações atuais. 

### Instalação do Material
No terminal / cmd digite:
```bush
pip install mkdocs-material 
```

Para mais detalhes sobre o tema acesse a página do [material para MKDocs]{{ links.github_material }} no [Github]{{ links.github }}

# Plugins
## MKDocs macros
O MKDcos macros permite a criação de variáveis no arquivo **mkdocs.yml** do [MKDocs]({{ links.mkdocs }}) para facilitar futuras manutenções.

### Instalação
No terminal / cmd digite:
```bush
pip install mkdocs-macros-plugin
```

### Utilização
```yaml
extra:
    nome_grupo:
        nome_variavel: valor_variavel
```

```yaml
extra:
    nomes:
        perfil_viga: perfil U 
```

Referência:
```bush 
O {{ links.perfil_viga }}
```

Resultado:
```bush
O perfil U...
```

## pymdown-extension
O pymdown extension é utilizado para disponibilizar os recursos de {{ links.markdown }} expandido, como ==texto realçado==, ~texto tachado~, [] ToDo list, entre outros recursos.

## Instalação
No terminal / cmd digite:
```bush
pip install mdown-extension-plugin
```

### Utilização
Para adicionar os recursos desejados, no arquivo .yml, no grupo markdown_extensions, adicione os recursos desejados.
Para consulta dos recursos e mais informações acesse a [documentação do PyMDown Exntensions]({{ links.pymdown_extensions }})

## MKDocs Collouts
O MKDocs Collauts habilita caixas de texto destacadas

>[!info]
> Use > para iniciar o bloco destacado

>[!warning] Atenção
>Exemplo de callout

Para mais detalhes, acesse a documentação do (MKDocs Collouts)[{{ links.mkdocs_collouts }}]

# Disponibilar a documentação online
Todos os arquivos referentes a documentação estão disponíveis no repositório [documentacao_gimi]({{ links.github_doc_repo }}) do [github]({{ links.github }}).

Após qualquer atualização ou ao fim do dia de trabalho é recomendado o upload da documentação no repositório do [github]({{ links.github }}).

O [repositório do projeto]({{ links.github_doc_repo }}) está vinculado com o [netlify]({{ links.netlify }}), um site de hospedagem de sites estáticos, onde a documentação pode ser acessada por qualquer dispositivo.

## Atualização da documentação
