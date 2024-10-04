# Perfil produtivo
## Criar montagem por família
- Crie uma montagem para cada família de peça.
- Salve a montagem na pasta da família na pasta de peças com o nome da família seguido de `_`.

{{ imagens.inventor_montagem_perfil_produtivo}}

- Insira todas as peças da família na montagem.

{{ imagens.inventor_arquivos_montagem_perfil_produtivo }}

## Criar montagem geral
- Crie uma montagem na pasta _Submontagem_.
- Nomeie a montagem como _"TODAS AS PEÇAS"_.

{{ imagens.inventor_arquivos_todas_as_pecas_perfil_produtivo }}

- Insira todas as submontagens das famílias criadas na seção [Criar montagem por família](#criar-montagem-por-família).

## Gerar o checklist de peças (BOM_P)
- Na submontagem geral, na aba _Assemble_, na seção _Manage_ clique em _Bill of materials_.

{{ imagens.inventor_Assemble_bill_of_materials }}

- Na janela _Bill of materials_ clique em _Import_.

{{ imagens.inventor_bill_of_materials_bill_of_materials }}

- Selecione o arquivo _{{ inventor.nome_conf_descricao }}_ em _{{ inventor.caminho_conf_descricao }}_.

{{ imagens.inventor_bill_of_materials_conf_descricao }}

- CLique em Sort Itens.

{{ imagens.inventor_bill_of_materials_sort_itens }}

- Em _Sort by_ selecione a opção _Description_.
- Em _Then by_ selecione a opção _Part Number_.

{{ imagens.inventor_sort_itens_sort }}

- Clique em _Export Bill of Materials.

{{ imagens.inventor_export_bill_of_materials }}

- Selecione o caminho onde o arquivo será salvo.

## Cadastro de peças
- Abra o arquivo _BOM_P_ criado na seção [Gerar o checklist de peças (BOM_P)](#gerar-o-checklist-de-peças-bom_p).
- Selecione toda a tabela sem o cabeçalho e sem a coluna "**_Item_**"

{{ imagens.excel_colunas_perfil_produtivo }}

- Copie os itens e cole na tabela de perfil produtivo