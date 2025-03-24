## Objetivo
A nomenclatura adotada como padrão tem como objetivo facilitar a identificação das características da peça ou conjunto apenas pelo código.

## Codificação
### Peças, montagens e submontagens
O código das peças e conjuntos padronizados são compostos da seguinte estrutura:

<p style="text-align:center; font-weight:bold"> AA.B.CC.000.00.XY </p>

AA - [Produto](#tabela-aa-produto)
B - [Aplicação](#tabela-b-aplicacao)
CC - [Família](#tabela-cc-familia)
000 - Número sequencial
00 - Número da variável
X - [Material](#tabela-x-material)
Y - [Bitola](#tabela-y-bitola)

> [!exemplo] Exemplo:
> <p style="text-align:center; font-weight:bold"> NP.P.BA.001.01.BA </p>
> **Produto:** New Piccolo
> **Aplicação:** Peça
> **Família:** Base
> **Sequência:** 001
> **Variável:** 01
> **Material:** NBR 7008 ZC
> **Bitola:** #12

As peças específicas para a obra seguem o seguinte padrão:

<p style="text-align:center; font-weight:bold"> AA.B.CC.000.00.XY-OBRA </p>

AA - [Produto](#tabela-aa-produto)
B - [Aplicação](#tabela-b-aplicacao)
CC - [Família](#tabela-cc-familia)
000 - Número sequencial
00 - Número da variável
X - [Material](#tabela-x-material)
Y - [Bitola](#tabela-y-bitola)
OBRA - Número da obra (E-XXXX)

As siglas usadas em cada campo pode ser consultada nas tabelas abaixo

### Barramento
O código dos barramentos padronizados são compostos da seguinte estrutura:

<p style="text-align:center; font-weight:bold"> AA.B.CC.000.00.XYD </p>

AA - [Produto](#tabela-aa-produto)
B - [Aplicação](#tabela-b-aplicacao)
CC - [Família](#tabela-cc-familia)
000 - Número sequencial
00 - Número da variável
X - [Material](#tabela-x-material)
Y - [Bitola](#tabela-y-bitola) - Tipo de barra
D - [Fase](#tabela-d-fase)

> [!exemplo] Exemplo:
> <p style="text-align:center; font-weight:bold"> ART.B.BG.001.01.DEA </p>
> **Produto:** Armário ao tempo
> **Aplicação:** Barramento
> **Família:** Barramento geral
> **Sequência:** 001
> **Variável:** 01
> **Material:** Cobre
> **Bitola:** 25x5
> **Fase:** Aterramento

### Base de {{ nomes.perfil_viga }}
<p style="text-align:center; font-weight:bold"> AA.B.CC.112.00.X </p>

AA - [Produto](#tabela-aa-produto)
B - [Aplicação](#tabela-b-aplicacao)
CC - [Família](#tabela-cc-familia)
11 - [Utilização da base](#tabela-11-utilizacao-da-base)
2 - [Especificação](#tabela-2-especificacao)
00 - Número da variável
X - [Material](#tabela-x-material)

> [!exemplo]Exemplo:
> <p style="text-align:center; font-weight:bold"> SK.S.BA.002.01.I </p>
> **Produto:** Skid
> **Aplicação:** Submontagem
> **Família:** Base
> **Utilização da base**: Base para inversores
> **Especificação:** 2 inversores
> **Variável:** 01
> **Material:** ASTM A36

### Tabela AA - Produto
| Sigla | Produto | Classe de tensão |
| :---: | :-----: | :--------------: |
| AR | Armário | Baixa |
| NU | Cabine de barramento | Baixa |
| QE | Quadro de embutir | Baixa |
| QS | Quadro de sobrepor | Baixa |
| CM | Caixa de medição | Média |
| CV | Convencional | Média |
| CT | Cubículo de transformador | Média |
| DO | Disjuntor On board | Média |
| IN | Invólucro | Média |
| MG | Maggiore | Média |
| MC | Microcompact | Média |
| MC36 | Microcompact 36 kV | Média |
| NP | New Piccolo | Média |
| SI | Simplificada | Média |
| SK | Skid | Média |

### Tabela B - Aplicação
| Sigla | Aplicação |
| :---: | :-------: |
| M | Montagem |
| P | Peça |
| S | Submontagem |

### Tabela CC - Família
| Sigla | Família |
| :---: | :-----: |
| BA* | Barramento de aterramento |
| BD | Barramento de derivação |
| BG | Barramento geral |
| BI | Barramento de interligação |
| BN* | Barramento de neutro |
| BA* | Base |
| BT | Batente |
| CC | Caixa de comando |
| CT | Caixa de transição |
| CX | Caixa |
| CH | Chapéu |
| CL | Coluna |
| ES | Estrutura |
| FE | Fechamento externo |
| FI | Fechamento interno |
| FL | Flange |
| PM | Placa de montagem |
| PE | Porta |
| RE | Reforço |
| SU | Suporte |
| TE | Tela |

\* Para saber a qual família o código se refere verifique a [Aplicação](#tabela-b-aplicacao).

### Tabela X - Material
| Sigla | Material |
| :---: | :------: |
| A | SAE 1008 |
| B | NBR 7008 ZC |
| C | NBR 7008 PRÉ PINTADO |
| D | COBRE |
| E | ALUMÍNIO |
| F | POLICARBONATO |
| G | FIBRA DE VIDRO |
| H | CELERON |
| I | ASTM A36 |

### Tabela Y - Bitola
| Sigla | Bitola chapa | Barramento - Tipo |
| :---: | :----: | :--------------------: |
| A | 12 | 12x3 - Canto vivo |
| B | 14 | 20x3 - Arredondado |
| C | 16 | 25x3 - Arredondado |
| D | 20 | 20x5 - Canto vivo |
| E | -- | 25x5 - Canto vivo |
| F | -- | 40x5 - Canto vivo |
| G | -- | 50x5 - Canto vivo |
| H | -- | 60x5 - Canto vivo |
| I | -- | 80x5 - Canto vivo |
| J | -- | 100x5 - Canto vivo |
| K | -- | 125x5 - Canto vivo |
| L | -- | 25x6 - Arredondado |
| M | -- | 40x6 - Arredondado |
| N | -- | 30x10 - Canto vivo |
| O | -- | 40x10 - Canto vivo |
| P | -- | 40x10 - Arredondado |
| Q | -- | 50x10 - Canto vivo |
| R | -- | 60x10 - Canto vivo |
| S | -- | 80x10 - Canto vivo |
| T | -- | 80x10 - Arredondado |
| U | -- | 100x10 - Canto vivo |
| V | -- | 120x10 - Canto vivo |
| W | -- | 160x10 - Canto vivo |
| X* | -- | $\frac{3}{8}$" x $\frac{3}{32}$" - Canto vivo * |

\* Barramentos em polegada
- Demais barramentos em milímetros

### Tabela Z - Tipo de chapa
| Sigla | Bitola |
| :---: | :----: |
| F | COMUM |
| Z | ZINCADA |

### Tabela D - Fase
| Sigla | Fase |
| :---: | :--: |
| A | RS |
| B | ST |
| C | RT |
| D | RST |
| E | RSTN |
| N | Neutro |
| P | Terra |
| R | R |
| S | S |
| T | T |

### Tabela 11 - Utilização da base
| Numeração | Utilização |
| :-------: | :--------: |
| 00 | Inversores |
| 01 | Transformador |
| 02 | Transformador + Armário |
| 03 | Cabine primária + Transformador |
| 04 | Cabine primária + Transformador + Armário |
| 05 | Cabine primária |
| 06 | Armário + Inversores |

### Tabela 2 - Especificação
> [!warning] Base com inversores
> Para base de inversores utilizar a quantidade de inversores

| Numeração | Especificação |
| :-------: | :-----------: |
| 0 | Transformador a seco |
| 1 | Transformador a óleo |
| 2 | Transformador a seco e óleo |
| 3 | Transformador a óleo com contenção |