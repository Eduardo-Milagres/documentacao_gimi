# Opções de aplicação GIMI
"*Application Options*" é uma ferramenta que configura todas as opções do software, como a cor da tela de fundo, aparência, qualidade de imagem, tempo de resposta ao fazer uma ação, locais de salvar bibliotecas, templates, etc. Por tanto trata-se de configurações importantes, onde todos os computadores devem ter as mesmas configurações.

## Setup do Opções de aplicação GIMI (Operadores)
Após a instalação do software, para configurar o "*Application Options*" da GIMI é necessário os seguintes passos:

1. Clique na aba *tools* na faixa de ferramentas.

==imagem==

2. No grupo *Options* clique em *Application Options*

==imagem==

>[!warning] Importante
>   Esta importação deve ser feita nos seguintes casos:
>   - Pós instalação do Inventor
>   - Erro de banco de dados
>   - Sincronização de todas as máquinas
>   O arquivo de *Application Options* nunca deve ser duplicado

## Edição do Opções de aplicação GIMI (Manager)
### Aba "General"
==imagem==

#### Grupo "*Startup*"
##### "*Startup action*"
Quando ativado, nos permite 3 opções ao abrir o inventor.

1. "*File Open dialog*": Ao abrir o Inventor, abre-se uma janela pedindo algum arquivo;
2. "*File New Dialog*": Ao abrir o Inventor, abre-se a janela "*Create New File*" para criar um novo arquivo.
3. "*New from tamplate*": Ao abrir o Inventor, abre-se uma janela de tamplate.

##### "*Show My Home on Startup*"
Quando ativado deixa a área *Home* ativa.

#### Grupo "*Prompting Interaction*"
1. "*Show command prompting (Dynamic Prompts)*"
2. "*Show command alias input dialog*"

#### Grupo "*Tooltip Appearance*"
==Preencher==

### Aba "File"
#### Campo "*Undo*"
Caminho para a pasta de arquivos temporários onde o Inventor busca as referências ao utilizar o comando _Undo_ (Desfazer: Ctrl + Z).

```bush
{{ inventor.caminho_applicationOptions_file_undo }}
```

#### Campo "*Default Templates*"
Caminho para a pasta de templates onde o Inventor busca as referências para a criação de arquivos baseados no padrõa estabelecido.

```bush
{{ inventor.caminho_applicationOptions_file_defaultTemplate }}
```

#### Campo "*Design Data*"
Caminho para a pasta de configuração da aba _Design-Inventor_.

```bush
{{ inventor.caminho_applicationOptions_file_designData }}
```

#### Campo "*Sketch Symbol Library Folder*"
Caminho para a pasta de biblioteca de simbolos.

```bush
{{ inventor.caminho_applicationOptions_file_sketchSymbolLibraryFolder }}
```

#### Campo "*Default Content Center Files*"
Caminho para a pasta de elementos de máquina (Content Center).

```bush
{{ inventor.caminho_applicationOptions_file_defaultContentCenter }}
```

#### Campo "*Project Folder*"
Caminho onde serão salvos os atalhos dos _Projects_ (.ipj) criados.

```bush
{{ inventor.caminho_applicationOptions_file_projectsFolder }}
```

### Aba "Drawing"
==imagem==

### Aba "Parts"
==imagem==

### Aba "Assembly"
==imagem==

### Aba "Content Center"
==imagem==