# Elaboração da base
## 1. Criação do esqueleto (.ipt)
1.1 Crie uma nova peça e salve na pasta _MONTAGEM/BASE_ com o nome de acordo com a [nomenclatura](../Nomenclatura.md) e _"-ESQUELETO"_ após o nome.
1.2 Crie um Sketch e selecione o plano de trabalho desejado
1.3 Desenho o layout da base 
{{ imagens.inventor_esqueleto_ipt }}

## 2. Criação da montagem (.iam)
> [!tip] Dica
> Crie o arquivo de montagem com solda pois na etapa de simulação será necessário.
2.1. Inserir o esqueleto na montagem

## 3. Insirer as vigas em "{{ nomes.perfil_viga }}"
- Na aba _Design_ clique em _Insert Frame_
{{ imagens.inventor_design_insert_frame }}

- Na janela _Insert_, selecione o perfil da viga.
{{ imagens.inventor_insert_frame_insert}}

>[!info] Perfis utilizados
> *Standart*: {{ inventor.norma_viga }}
> *Family*: {{ inventor.familia_viga }}
> *Size*: 3x200x50, 4.75x200x50 ou 3x75x38
> *Material*: {{ inventor.material_viga }}

- Selecione as linhas do esqueleto para referência da viga.
{{ imagens.inventor_insert_frame_seleção_linhas_guia }}

- Na janela, no grupo _Orientation_ selecione a orientação da viga, conforme a pré visualização.
- Clique em _Apply_ para criar as vigas.

- Na janela _Create New Frame_, clique no ícone da pasta em _New Frame File Location_ e salve o arquivo na pasta _SUBMONTAGEM/BASE_ com o nome de acordo com a codificação de montagem, vide [nomenclatura](../Nomenclatura.md).
- Clique no ícone da pasta em _New Skeleton File Name_ e salve o arquivo em SUBMONTAGEM/BASE. O nome do arquivo do esqueleto deve ser o mesmo da estrutura seguido de "-ESQUELETO".

>[!exemplo] Exemplo
>Nome da estrutura: _{{ geral.codigo_montagem_frame }}_
>Nome do esqueleto: _{{ geral.codigo_esqueleto_frame }}_
  
{{ imagens.inventor_insert_frame_create_new_frame }} 
{{ imagens.inventor_insert_frame_create_new_frame_nome_montagem }}
{{ imagens.inventor_insert_frame_create_new_frame_nome_esqueleto }}

## 4. Nomear e Salvar as peças das vigas 
- Na caixa de diálogo clique no caminho da peça e em seguida no botão indicado abaixo para abrir o explorador de arquivos.

{{ imagens.inventor_frame_member_naming }}
- Salve as vigas em _PEÇAS/BASE_ com a codificação seguindo o padrão de [nomenclatura](../Nomenclatura.md) de peças.

>[!exemplo] Exemplo
>SK.P.BA.001.01.I

{{ imagens.inventor_frame_member_naming_nome }}

### Padronização da nomenclatura da base
#### Vigas do contorno ({{ inventor.nome_viga_contorno }})
- Para as vigas do contorno da base utilize o padrão de nomenclatura _{{ inventor.nome_viga_contorno }}_ alterando somente a variável (XX).

{{ imagens.inventor_nomenclatura_viga_contorno }}

#### Vigas longitudinais ({{ inventor.nome_viga_longitudinal }})
- Para as vigas longitudinais da base utilize o padrão de nomenclatura _{{ inventor.nome_viga_longitudinal }}_ alterando somente a variável (XX).

{{ imagens.inventor_nomenclatura_viga_longitudinal }}

#### Vigas para apoio ({{ inventor.nome_viga_apoio }})
- Para as vigas de apoio dos fechamento e canaletas da base utilize o padrão de nomenclatura _{{ inventor.nome_viga_apoio }}_ alterando somente a variável (XX).

{{ imagens.inventor_nomenclatura_viga_apoio }}

#### Vigas tranversais ({{ inventor.nome_viga_transversal }})
- Para as vigas transversais da base utilize o padrão de nomenclatura _{{ inventor.nome_viga_transversal }}_ alterando somente a variável (XX).

{{ imagens.inventor_nomenclatura_viga_transversal }}

## 5. Encaixes
### Milter
- Para realizar o encaixe das vigas da extremidade, use o comando _Milter_ na guia _Design_.

{{ imagens.inventor_design_milter }}

{{ imagens.inventor_encaixe_vigas_antes_milter }} {{ imagens.inventor_encaixe_vigas_depois_milter }}

### Trim / Extend
- Com excessão das vigas do contorno externo, todas as vigas devem ser extendidas para garantir o contato entre elas.
- Para extender as vigas, na aba _3D Model_ clique em _Trim/Extend_.
  
{{ imagens.inventor_design_trim_extend }}

- Selecione a viga a ser extendida e depois a face até onde a viga será extendida.

  {{ imagens.inventor_viga_antes_trim_extend }}{{ imagens.inventor_trim_extend }}

### Vigas internas
- Vigas internas são aquelas que se encaixam entre as abas de outras vigas
#### Chanfro
- Para realizar o encaixe das vigas fixadas na parte interna de outras vigas abra a peça, na aba _3D Model_ clique em _Chamfer_.

{{ imagens.inventor_3Dmodel_chamfer }}

- Na janela _Chamfer_ clique na seta para expandir a caixa de diálogo.
- Selecione a opção _Single Edge_.

{{ imagens.inventor_chamfer_chamfer }}

- Selecione as lihas a serem chamfradas.

>[!info] Distância do chamfro
> Vigas com 75 mm de largura: {{ geral.chanfro_viga_75 }}
> Vigas com 200 mm de largura: {{ geral.chanfro_viga_200 }}

{{ imagens.inventor_viga_antes_chanfro }}{{ imagens.inventor_viga_depois_chanfro }}

#### Notche
- Para realizar o encaixe das vigas fixadas na parte interna de outras vigas use o comando _Notche_ na guia _Design_.

{{ imagens.inventor_design_notche }}

{{ imagens.inventor_encaixe_vigas_antes_notche }}{{ imagens.inventor_viga_depois_chanfro }}
{{ imagens.inventor_encaixe_vigas_depois_notche }}{{ imagens.inventor_viga_depois_notche_peça }}

## 6. Detalhamento
