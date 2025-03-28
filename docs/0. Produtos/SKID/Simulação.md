# Simulação da base
## 1. Desativar o cncCAD_{{ geral.cad_link_version }}
- Na aba _Tools_ no grupo _Optins_ clique em _Add-ins_.

{{ imagens.inventor_tools_add_ins }}

- Na caixa de diálogo (Add-In Manager) no grupo _Load Behavior_ marque apenas a opção _Block_ e clique em _OK_.

{{ imagens.inventor_add_ins_manager }}

## 2. Criando a simulação
- Na aba _Envioronments_ clique em _Stress Analysis_.

{{ imagens.inventor_stress_analysis }}

- Na aba _Stress Analysis_ clique me _Create Simulation_.

{{ imagens.inventor_create_simulation }}

- Na caixa de diálogo pode-se alterar as configurações de tolerância, porém as definições padrães atentem as exigências.
- Clique em _OK_ para criar a simulação.

{{ imagens.inventor_create_new_simulation }}

## 3. Definindo os materiais
- Na aba _Stress Analysis_ clique em _Assign_.

{{ imagens.inventor_assign }}

- Na caixa de diálogo (Assign Materials) clique na primeira linha da coluna _Override Material_, segure a tecla _Shift_ e clique na última linha da coluna _Override Material_.
- Clique na seta indicada e defina o material como {{ inventor.material_viga }} e clique em _OK_.

{{ imagens.inventor_assign_materials }}

## 4. Definindo as restrições
- Na aba _Stress Analysis_ cliqeu em _Fixed_.

{{ imagens.inventor_fixed }}

- Selecione o ponto de apoio do olhal e clique em _Apply_.
  
>[!warning] Atenção
> As faces devem ser selecionadas individualmente para que os resultados de esforços no relatórios sejam apresentados individualmente, vacilitando a análise.

{{ imagens.inventor_fixed_constraint }}

## 5. Definindo as cargas
### Gravidade
- Na aba _Stress Analysis_ clique em _Gravity_.

{{ imagens.inventor_gravity }}

- Selecione qualquer face paralela ao piso e clique em _OK_.

{{ imagens.inventor_gravity_gravity }}

### Cargas aplicadas
>[!warning] Atenção
> Se a simulação for feita utilizando os blocos que simulam as massas sobre a base, não é necessário aplicar outras cargas.

- Na aba _Stress Analysis_ clique em _Force_.

{{ imagens.inventor_force }}

- Selecione a face onde a força será aplicada e no campo magnitude digite a intensidade da carga em Newtons (N).

{{ imagens.inventor_force_force }}

>[!tip] Dica
> Para facilitar a identificação das forças, selecione uma cor diferente da cor utilizada na gravidade.

## 6. Criação da malha
- Na aba _Stress Analysis_ clique em _Mesh View_.

{{ imagens.inventor_mesh_view }}

## 7. Simulação
- Na aba _Stress Analysis_ clique em _Simulate_.

{{ imagens.inventor_simulate }}

- Verifique a caixa de erros, caso não tenha nenhum problema, clique em _Run_.

{{ imagens.inventor_simulate_simulate }}

## 8. Análise dos resultados
### Probe - Valores máximo e mínimo 
- Para visualizar os valores máximos e mínimos do resultado, na gui _Stress Analysis_ clique em _Maximum value_ para ver o valor máximo e em _Minimum value_ para ver o valor mínimo.

{{ imagens.inventor_maximum_minimum_value }}

{{ imagens.inventor_visualizacao_probe }}

### Probe - Personalizada
- Na guia _Stress Analysis_ clique em _Probe_.

{{ imagens.inventor_probe }}

- Selecione o ponto em que deseja visualizar o resultado.

{{ imagens.inventor_visualizacao_probe_customizada }}

### Von Misses Stress
- A tensão de Von Misses indica as tensões da estrutura.

>[!warning] Atenção
>O valor máximo de tensão não pode ultrapassar a tensão de escolamento do aço ($\sigma_{esc}$ = {{ geral.tensao_escoamento_A36 }}).

### Displacement
- Indica o deslocamento da estrutura.

>[!warning] Atenção
>O valor máximo de deslocamento não pode ser superior ao comprimento da viga divido por 300 ($\frac{Comp. \, viga}{300}$), conforme NBR 8800.

### Safety factor
- Indica o fator de segurança da estrutura em relação a tensão de escoamento do material ($\sigma_{esc}$).
- O valor é obtido pela razão entre a tensão de escoamento do material ($\sigma_{esc}$) e a tensão máxima de Von Misses ($\sigma_{máx}$).

>[!warning] Atenção
> Valores abaixo de 1 indicam que a estrutura não suportara as cargas aplicadas e entrará em colpso.

$$ FS = \frac{\sigma_{esc}}{\sigma_{máx}}$$

### Centro de gravidade (Baricentro)
- É o ponto geométrico onde a força peso é aplicada.

>[!warning] Atenção
>Para içamento é importante que o centro de gravidade esteja o mais centralizado possível com os olhais de içamento.

- Na aba _View_ clique em _Centro de Gravidade_

{{ imagens.inventor_view_center_of_gravity }}

{{ imagens.inventor_view_center_of_gravity_visualizacao }}

## 9. Gerar o relatório
- Na guia _Stress Analysis_ clique em _Report_.

{{ imagens.inventor_report }}

- Na janela _Report_ em _Report Title_ altere o título do relatório.
- Desmarque a caixa de seleção do logo.
- No campo _Summary_ adicine os comentários necessários.

>[!tip] Dica
> Para o SKID é recomendado adicionar no campo _Summary_ as massas dos blocos e o modelo do transfordor.

- No grupo _Report Location_ em _Filename_ digite o nome desejado para o arquivo do relatório.

{{ imagens.inventor_report_report }}


- Em _Path_ clique em `...` e selecione o local onde o relatório sera salvo.

{{ imagens.inventor_report_report_path }}

### 9.1. Esforço nos olhais
>[!warning] Carga máxima dos olhais
>Conforme os ensaios dos olhais de içamento, cada olhal suporte até {{ geral.carga_maxima_olhal_skid }} de carga.

- Para garantir a integridade dos olhais durante o içamento, no relatório é necessário verificar a carga total aplicada em cada olhal.

- Na seção _Results_ do relatório, na coluna _Reaction Force_ verifique a magnitude para cada ponto de fixação. A magnitude máxima não deve ultrapassar a carga máxima suportada pelo olhal.

{{ imagens.inventor_report_results }}

