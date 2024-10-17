# Perfil produtivo
## 1. Criar a planilha de perfil produtivo
- Entre em [Perfil produtivo]({{ links.drive_pasta_perfil_produtivo }}) ({{ links.drive_pasta_perfil_produtivo }})
- Clique com o botão direito sobre o arquivo _PP - Template_.
- Clique em _Fazer uma cópia_.

{{ imagens.drive_fazer_uma_copia }}

- Clique com o botão direito sobre o arquivo criado "_Cópia de PP - Template_".
- Clique em _Renomear_ ou utilize o atalho ++ctrl+alt+e++.

{{ imagens.drive_renomear }}

- Renomeie o arquivo como `PP - Nome do Produto`.

{{ imagens.drive_exemplo_perfil_produtivo }}

### 1.1 Habilitar permissões
- Na aba _Configurações_, nas células com erro de referência `#REF!`, clique na célula e permita o acesso.

{{ imagens.sheets_perfil_produtivo_configurações_permitir_acesso }}

## 2. Criar montagem por família
- Crie uma montagem para cada família de peça.
- Salve a montagem na pasta de peças da família com o nome da família seguido de `_`.

{{ imagens.inventor_montagem_perfil_produtivo}}

- Insira todas as peças da família na montagem.

{{ imagens.inventor_arquivos_montagem_perfil_produtivo }}

## 3. Criar montagem geral
- Crie uma montagem na pasta _Submontagem_.
- Nomeie a montagem como _"TODAS AS PEÇAS"_.

{{ imagens.inventor_arquivos_todas_as_pecas_perfil_produtivo }}

- Insira todas as submontagens das famílias criadas na seção [Criar montagem por família](#criar-montagem-por-família).

## 4. Gerar o checklist de peças (BOM_P)
- Na submontagem geral, na aba _Assemble_, na seção _Manage_ clique em _Bill of materials_.

{{ imagens.inventor_Assemble_bill_of_materials }}

- Na janela _Bill of materials_ clique em _Import_.

{{ imagens.inventor_bill_of_materials_bill_of_materials }}

- Selecione o arquivo _{{ inventor.nome_conf_descricao }}_ em _{{ inventor.caminho_conf }}_.

{{ imagens.inventor_bill_of_materials_conf_descricao }}

- Clique em Sort Itens.

{{ imagens.inventor_bill_of_materials_sort_itens }}

- Em _Sort by_ selecione a opção _Description_.
- Em _Then by_ selecione a opção _Part Number_.

{{ imagens.inventor_sort_itens_sort }}

- Clique em _Export Bill of Materials_.

{{ imagens.inventor_export_bill_of_materials }}

- Selecione o caminho onde o arquivo será salvo.

## 5. Cadastro de peças
- Abra o arquivo _BOM_P_ criado na seção [Gerar o checklist de peças (BOM_P)](#gerar-o-checklist-de-peças-bom_p).

- Na seção _Edição_ clique em _Localizar e selecionar_ e selecione a opção _Susbtituir_ ou utilize o atalho ++ctrl+u++.

{{ imagens.excel_edicao_localizar_e_substituir }}

- Em _Localizar_ digite `"espaço" mm` e deixe o campo _Substituir por_ em branco.
- Clique em _Substituir tudo_.
- Em _Localizar_ digite `"espaço" kg` e deixe o campo _Substituir por_ em branco.
- Clique em _Substituir tudo_.

{{ imagens.excel_localizar_e_selecionar_substituir }}

- Selecione toda a tabela sem o cabeçalho e sem a coluna "**_Item_**"

{{ imagens.excel_colunas_perfil_produtivo }}

- Copie os itens selecionados
- Cole na tabela de perfil produtivo na guia _Peças_ da planilha gerada na etapa [1. Criar planilha de perfil produtivo](#1-criar-a-planilha-de-perfil-produtivo).

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_peças}}

## 6. Cadastro de submontagens
- Abra o arquivo de submontagem no _Autodesk Inventor_. 
- Na aba _Assemble_, na seção _Manage_ clique em _Bill of materials_.

{{ imagens.inventor_Assemble_bill_of_materials }}

- Na janela _Bill of materials_ clique em _Import_.

{{ imagens.inventor_bill_of_materials_bill_of_materials }}

- Selecione o arquivo _{{ inventor.nome_conf_quant }}_ em _{{ inventor.caminho_conf }}_.

{{ imagens.inventor_bill_of_materials_conf_quant }}

- Clique em Sort Itens.

{{ imagens.inventor_bill_of_materials_sort_itens }}

- Em _Sort by_ selecione a opção _Description_.
- Em _Then by_ selecione a opção _Part Number_.

{{ imagens.inventor_sort_itens_sort }}

- Copie os valores sem a coluna **_Item_**.

{{ imagens.inventor_bill_of_materials_colunas_submontagem }}

- Cole na tabela de perfil produtivo na guia _Kits_, na coluna _Composição_ da planilha gerada na etapa [1. Criar planilha de perfil produtivo](#1-criar-a-planilha-de-perfil-produtivo).

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_kits_submontagem }}

- Na coluna _Submontagem_ insira o nome da submontagem que está sendo cadastrada.

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_kits_submontagem_nome }}

- Na coluna _Família_ insira o nome da família que está sendo cadastrada.

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_kits_submontagem_familia }}

## 7. Cadastro de montagens
- Abra o arquivo de montagem no _Autodesk Inventor_. 
- Na aba _Assemble_, na seção _Manage_ clique em _Bill of materials_.

{{ imagens.inventor_Assemble_bill_of_materials }}

- Na janela _Bill of materials_ na guia _Structure_, clique em _Import_.

{{ imagens.inventor_bill_of_materials_structure }}

- Selecione o arquivo _{{ inventor.nome_conf_quant }}_ em _{{ inventor.caminho_conf }}_.

{{ imagens.inventor_bill_of_materials_conf_quant }}

- Clique em Sort Itens.

{{ imagens.inventor_bill_of_materials_sort_itens }}

- Em _Sort by_ selecione a opção _Description_.
- Em _Then by_ selecione a opção _Part Number_.

{{ imagens.inventor_sort_itens_sort }}

- Copie os valores sem a coluna **_Item_**.

>[!warning] Atenção
> Não selecione as linhas com elementos de máquinas e itens de biblioteca.

{{ imagens.inventor_bill_of_materials_structure_colunas }}

- Cole na tabela de perfil produtivo na guia _Kits_, na coluna _Composição_ da planilha gerada na etapa [1. Criar planilha de perfil produtivo](#1-criar-a-planilha-de-perfil-produtivo).

- Na coluna _Submontagem_ insira o nome da submontagem que está sendo cadastrada.

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_kits_submontagem_nome }}

- Na coluna _Família_ insira o nome da família que está sendo cadastrada.

{{ imagens.sheets_perfil_produtivo_exemplo_tabela_kits_submontagem_familia }}

## 8. Elementos de máquina
### 8.1 Cadastro de novos elementos de máquina
- Todos os elementos de máquinas utilizados nos perfis produtivos estão centralizados na planilha [CD - Elementos de máquina]({{ links.drive_cd_elementos_maquina }}).

- Na coluna _Descrição_ adicione a nomenclatura de acordo com o elemento.
- Na coluna _Código_ adicoine o código iAPP do elemento.

{{ imagens.sheets_CD_elementos_máquina_exemplo }}

### 8.2 Cadastro dos elementos de máquinas nos Kits
- Na aba _Kits_, na coluna _Composição_ adicione os elementos de máquina conforme cada submontagem.
- Na coluna _Quant. (un.)_ ensira a quantidade usada no item cadastrado para cada elemento de máquina.

{{ imagens.sheets_perfil_produtivo_kits_elementos_maquina_exemplo }}