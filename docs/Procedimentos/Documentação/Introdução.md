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

### Material
O [material]({{ links.material }}) é um tema aplicado ao [MKDocs]({{ links.mkdocs }}) para alterar o layout das páginas e adicionar algumas funcionalidades. O [material]({{ links.material }}) é o tema mais utilizado nas documentações atuais. 

#### Instalação do Material
No terminal / cmd digite:
```bush
pip install mkdocs-material 
```

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
