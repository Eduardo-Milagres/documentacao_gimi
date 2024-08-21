# Elaboração da base
## 1. Criação do esqueleto (.ipt)
1.1 Crie uma nova peça e salve na pasta MONTAGEM/BASE_ com o nome de acordo com a [nomenclatura](../Nomenclatura.md) e _"-ESQUELETO"_ após o nome.
1.2 Crie um Sketch e selecione o plano de trablaho desejado
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

- Na janela, no grupo _Orientation_ selecione a orientação da viga, conforme a pré vizualição.
- Clique em _Apply_ para criar as vigas.

- Na janela _Create New Frame_, clique no ícone da pasta em _New Frame File Location_ e salve o arquivo na pasta _SUBMONTAGEM/BASE_ com o nome de acordo com a codificação de montagem, vide [Nomenclatura](../Nomenclatura.md).
- Clique no ícone da pasta em _New Skeleton File Name_ e salve o arquivo no mesmo local da montagem. O nome do arquivo do esqueleto deve ser o mesmo da estrutura seguido de "-ESQUELETO".

>[!exemplo] Exemplo
>Nome da estrutura: _SK.S.BA.002.01.IZ_
>Nome do esqueleto: _SK.S.BA.002.01.IZ - ESQUELETO_
  
{{ imagens.inventor_insert_frame_create_new_frame }} 
{{ imagens.inventor_insert_frame_create_new_frame_nome_montagem }}
{{ imagens.inventor_insert_frame_create_new_frame_nome_esqueleto }}

## 4. Encaixes
### Milter
- Para realizar o encaixe das vigas da extremidade, use o comando _Notche_ na guia _Design_.

{{ imagens.inventor_design_milter }}

{{ imagens.inventor_encaixe_vigas_antes_milter }} {{ imagens.inventor_encaixe_vigas_depois_milter }}

### Trim / Extend
- Com excessão das vigas do contorno externo, todas as vigas devem ser extendidas para garantir o contato entre elas.
- Para extender as vigas, na aba _3D Model_ clique em _Trim/Extend_.
  
{{ imagens.inventor_design_trim_extend }}

- Selecione a viga a ser extendida e depois a face até onde a viga será extendida.

  {{ imagens.inventor_viga_antes_trim_extend }}{{ imagens.inventor_trim_extend }}

### Vigas internas
#### Chanfro
- Para realizar o encaixe das vigas das vigas fixadas na parte interna de outras vigas abra a peça, na aba _3D Model_ clique em _Chamfer_.

>[!info] Distância do chamfro
> Vigas com 75 mm de largura: {{ geral.chanfro_viga_75 }}
> Vigas com 200 mm de largura: {{ geral.chanfro_viga_200 }}

{{ imagens.inventor_3Dmodel_chamfer }}

- Na janela _Chamfer_ clique na seta para expandir a caixa de diálogo.
- Selecione a opção _Single Edge_.

{{ imagens.inventor_chamfer_chamfer }}

- Selecione as lihas a serem chamfradas.

{{ imagens.inventor_viga_antes_chanfro }}{{ imagens.inventor_viga_depois_chanfro }}

#### Notche
- Para realizar o encaixe das vigas das vigas fixadas na parte interna de outras vigas use o comando _Notche_ na guia _Design_.

{{ imagens.inventor_design_notche }}

{{ imagens.inventor_encaixe_vigas_antes_notche }}{{ imagens.inventor_viga_depois_chanfro }}
{{ imagens.inventor_encaixe_vigas_depois_notche }}{{ imagens.inventor_viga_depois_notche_peça }}

## 5. Detalhamento
