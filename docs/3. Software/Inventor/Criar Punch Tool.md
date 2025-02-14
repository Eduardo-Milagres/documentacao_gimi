- Crie uma nova peça de chapa usando o template _Sheet Metal GIMI (mm).ipt_.

{{ imagens.inventor_create_new_file_sheet_metal_gimi_mm }}

- Salve a peça na pasta do componente ou para ferramentas na pasta _Parts_ na pasta raiz do _Punch Tool_.
```Z:\DOCUMENTO\Parametro\Punch Tool\Gimi```

- Crie uma face quadrada maior que a área total do _Punch Tool_ com a espessura igual a profundidade do _Punch Tool_.

{{ imagens.inventor_etapa_1_punch_tool }}

- Crie um _Sketch_ na face criada.

- Coloque um ponto no local de referência para inserção do _Punch Tool_.

{{ imagens.inventor_etapa_2_punch_tool }}

- No mesmo _Sketch_ do ponto faça o desenho com o perfil do _Punch Tool_.

{{ imagens.inventor_etapa_3_punch_tool }}

- Na aba _Sketch_, no grupo _Exit_, clique em _Finish Sketch_.

{{ imagens.inventor_sketch_finish_sketch }}
  
- Na aba _3D Model_, no grupo _Create_, clique em _Extrude_.

{{ imagens.inventor_3d_model_extrude }}

- Selecione os corpos do desenhos a serem extrudados.

{{ imagens.inventor_3d_model_extrude_extrude }}

- Na aba _Manage_, no grupo _Author_, clique em _Extract iFeature_.

{{ imagens.inventor_manage_extract_ifeature }}

- Selecione a opção _Sheet Metal Punch iFeature_.

{{ imagens.inventor_manage_extract_ifeature_sheet_metal_punch_ifeature }}

- Na árvore do modelo clique na _feature_ da extrusão criada anteriormente.

{{ imagens.inventor_etapa_4_punch_tool }}

- Clique com o botão direito em iFeature e selecione a opção _Rename_.

{{ imagens.inventor_etapa_5_punch_tool }}

- Digite o nome que aparecerá na árvore quando o _Punch Tool_ for utilizado.

>[!warning] Atenção
>O nome não pode conter caracteres especiais e/ou espaços.
>Substitua os espaços por "_".

- Clique em _Save_.

{{ imagens.inventor_manage_extract_save }}

- Selecione o local onde será salvo o _Punch Tool_.