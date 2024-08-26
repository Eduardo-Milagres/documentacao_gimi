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
> <p style="text-align:center; font-weight:bold"> SK.S.BA.002.00.IZ </p>
> **Produto:** Skid
> **Aplicação:** Submontagem
> **Família:** Base
> **Utilização da base**: Base para inversores
> **Especificação:** 2 inversores
> **Variável:** 01
> **Material:** ASTM A36
> **Tipo de chapa:** Zincada

### Tabela AA - Produto
| Sigla | Produto | Classe de tensão |
| ----- | ------- | ---------------- |
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
| ----- | -------- |
| M | Montagem |
| P | Peça |
| S | Submontagem |

### Tabela CC - Família
| Sigla | Família |
| ----- | ------- |
| BA | Base |
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

### Tabela X - Material
| Sigla | Material |
| ----- | -------- |
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
| Sigla | Bitola |
| ----- | ------ |
| A | 12 |
| B | 14 |
| C | 16 |
| D | 20 |
| X | COBRE |

### Tabela Z - Tipo de chapa
| Sigla | Bitola |
| ----- | ------ |
| F | COMUM |
| Z | ZINCADA |

### Tabela 11 - Utilização da base
| Numeração | Utilização |
| ----- | ---------- |
| 00 | Inversores |
| 01 | Transformador |
| 02 | Transformador + Armário |
| 03 | Cabine primária + Transformador |
| 04 | Cabine primária + Transformador + Armário |
| 05 | Armário + Inversores |

### Tabela 2 - Especificação
> [!warning] Base com inversores
> Para base de inversores utilizar a quantidade de inversores

| Numeração | Especificação |
| ----- | ------ |
| 0 | Transformador a seco |
| 1 | Transformador a óleo |
| 2 | Transformador a óleo com contenção |