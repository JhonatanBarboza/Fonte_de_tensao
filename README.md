# SSC0180-Eletrônica
## Projeto: Fonte de Tensão Regulável 3v-12v (100mA)
Este projeto demonstra como converter uma voltagem de corrente alternada (AC) de 127V e 60Hz em uma voltagem contínua (DC) regulada entre 3V e 12V (100mA). Através da utilização de um transformador para redução inicial da voltagem, seguido por retificação usando diodos para converter AC em DC, e filtragem com um capacitor para suavizar a saída. A regulação adicional com um diodo Zener e um potenciômetro permite ajustar precisamente a voltagem de saída conforme necessário, garantindo um funcionamento confiável e estável do nosso sistema eletrônico.

## Componentes Eletrônicos
| Quantidade     | Componentes | Especificações | Valor |
| ---      | ---       | ---      | ---     |
| 1 | [Transformador Bivolt](https://www.radeleletronica.com.br/transformador-9-9v-2a-trafo-tr-02-009)  | 9V/18V     |  R$ 41,90   |
| 1 | [Ponte Retificadora](https://www.usinainfo.com.br/ponte-retificadora/ponte-retificadora-2w10-3938.html) | KBPC3510 | R$ 3,78 |
| 1     | [Capacitor](https://www.baudaeletronica.com.br/produto/capacitor-eletrolitico-470uf-16v-105c.html)        | 470uF / 50V     | R$ 4,27  |
| 1     | [Potenciômetro](https://www.magazineluiza.com.br/potenciometro-linear-5k-l20-jhs/p/kkjcfch767/cj/ptct/)        | Resistência: 5K  | R$ 6,74    |
| 4     | [Resistor 2k2](https://www.edfcomponentes.com.br/resistor/resistor-2k2-14w-5-2200-ohms-cr25)     | 2200 Ω 1/4W    | R$ 0,07  |
| 4     | [Resistor 1k8](https://www.proesi.com.br/resistor-carbono-1w-1k8)     | 1800 Ω 1/4W    | R$ 0,07  |
| 4     | [Resistor 4k4](https://www.ryndackcomponentes.com.br/resistor-4-3-5-1-4w-cr25-4r3-4-3r.html)     | 4400 Ω 1/4W    | R$ 0,07  |
| 1     | [Resistor 120 Ω](https://www.proesi.com.br/resistor-precisao-1-1-4w-120r)     | 120 Ω 1 W    | R$ 0,39   |
| 1     | [Diodo Zener](https://www.baudaeletronica.com.br/produto/diodo-zener-bzx55c-13v-05w.html)       | Diodo Zener BZX55C 13V/0,5W     |  R$ 0,49   |
| 1     | [LED Azul](https://www.eletrogate.com/led-alto-brilho-5mm-azul)       | 2V/20mA      | R$ 1,49    |
| 1     | [Transistor](https://www.proesi.com.br/bc368-transistor)       |  Transistor NPN - BC368      | R$ 0,43   |
| 1     | [Protoboard](https://www.wjcomponentes.com.br/protoboard-400)        | 400 furos    | R$ 20,00  |

Valor Total: R$ 59,91

### Vídeos do projeto funcionando

[video]


## Descrição dos Componentes
### Transformador: 
Um transformador é um dispositivo elétrico que altera os níveis de tensão em um circuito, baseado no princípio da indução eletromagnética descoberto por Michael Faraday. Em nosso projeto, utilizamos um transformador de 9+9 V para obter uma tensão de 18 V.

### Diodos:
Componentes elétricos que permitem o fluxo de corrente em uma única direção são utilizados no projeto para montar uma ponte de diodos. Essa ponte atua como um retificador de tensão, aproveitando ambos os ciclos da corrente alternada.

### Resistores:
Um resistor é um componente elétrico que limita o fluxo de corrente em um circuito. Ele dissipa energia na forma de calor e é utilizado para controlar níveis de tensão e corrente.  No nosso projeto foram utilizados resistores de 2k2, 1k8, 4k4 e um de 120.

### Capacitor:
Um capacitor é um componente eletrônico que armazena energia elétrica em um campo elétrico, composto por duas placas condutoras separadas por um material dielétrico. Ele é usado para filtrar sinais, estabilizar tensão e armazenar energia temporariamente. Em nosso projeto, ele foi utilizado para reduzir o ripple do sistema.

### Potenciômetro:
Componente com resistência ajustável que regula o fluxo de corrente e altera os níveis de tensão do circuito. Neste projeto, foi utilizado para selecionar os níveis de tensão entre 3V e 12V, conforme especificado.

### Diodo Zener:
Um diodo Zener é um tipo especial de diodo que permite o fluxo de corrente elétrica não só no sentido direto, mas também no sentido inverso quando a tensão aplicada ultrapassa um valor específico, chamado de tensão de Zener. Foi usado para garantir que a tensão ficasse abaixo de 13V no final do circuito, eliminando completamente o ripple. 

### Transistor:
Um transistor é um componente eletrônico semicondutor utilizado para amplificar ou comutar sinais elétricos. Ele possui três terminais: emissor, base e coletor, e opera controlando a corrente entre o coletor e o emissor através da corrente aplicada na base. Em nosso projeto, o transistor é empregado para controlar a amplificação de sinais e a comutação, essencial para o funcionamento eficiente do circuito.



## Conversão de Energia AC para DC Regulada

Neste projeto, o objetivo é converter um sinal elétrico de corrente alternada (AC) de 127V e 60Hz em uma voltagem contínua (DC) regulada entre 3V e 12V. Aqui estão os passos principais do processo:

### Transformação: 
Utilizamos um transformador para reduzir a alta voltagem AC de 127V para cerca de 19,5V, mantendo o formato da onda AC intacto.

### Retificação:
Os diodos retificadores convertem o sinal AC em um sinal DC positivo, permitindo que a corrente flua em apenas um sentido e eliminando os ciclos negativos da onda AC.

![retificação](https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/207acd34-a62c-4003-acb8-71223c2aec8b)

<sub>imagem 1

### Filtragem: 
Um capacitor é empregado para suavizar o sinal DC retificado, reduzindo as variações de voltagem (ripple) e produzindo uma saída mais estável.

![ripple-destaque-1](https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/d602ba6c-241b-4aac-9589-914851832a39)

<sub>imagem 2

### Regulação: 
Um diodo Zener é utilizado para fixar a voltagem em 13V, eliminando pequenas flutuações indesejadas na saída. Além disso, um potenciômetro é ajustado para permitir a seleção da voltagem final entre 3V e 12V conforme necessário.


## Cálculos

### Razão do Transformador

Para trabalhar com uma saída de tensão de Vs = 18V (medido na prática) e um transformador com uma razão de 8,5, usamos a equação do transformador para calcular a tensão de entrada necessária.

#### Tensão de Pico

Primeiramente, calculamos a tensão de pico V(pico) da entrada senoidal:

$$ V_{\text{pico}} = V_{\text{entrada}} \times \sqrt{2} $$

Onde:
- V(entrada) é a tensão de entrada da tomada (127V).

Substituindo os valores:

$$ V_{\text{pico}} = 127V \times \sqrt{2} = 179,6V $$

#### Razão do Transformador

Desejando um transformador que produza uma tensão de saída (Vs) de 18V com uma razão de 8,5, utilizamos a relação do transformador:

$$ \frac{1}{6,96} = \frac{V_s}{V_{\text{pico}}} $$

Resolvendo para V(s):

$$ V_s = \frac{V_{\text{pico}}}{8,5} $$

Substituindo os valores:

$$ V_s = \frac{179,6V}{8,5} \approx 21,1V $$

Considerando que o diodo precisa de uma tensão mínima de 0,7V cada, devemos subtrair 1,4V da tensão de saída:

$$ V_s = 25,8V - 1,4V = 19,7V $$

Portanto, a tensão de saída ajustada é de 19,7V.
##
### Cálculo da Tensão de Ripple (Vripple)

Para calcular a tensão de ripple, consideramos uma tensão de ripple de 10% da tensão de saída.

$$ V_{\text{ripple}} = 0,1 \times V_s $$

Substituindo o valor da tensão de saída:

$$ V_{\text{ripple}} = 0,1 \times 21,1V = 2,11V $$

Portanto, a tensão de ripple é 2,11V.
##
### Cálculo da Tensão Média

A tensão média V(média) é a média aritmética entre a tensão mínima e a tensão máxima, portanto:

1. **Identificação dos limites de variação**:
- Tensão mínima: 19,3V
- Tensão máxima: 19,7V

2. **Cálculo da Tensão Média**:
- A tensão média é calculada pela média aritmética entre V(min) e V (max):

$$ V_{\text{média}} = \frac{V_{\text{min}} + V_{\text{max}}}{2} $$

   Substituindo os valores conhecidos:

$$ V_{\text{média}} = \frac{19,3V + 19,7V}{2} $$

$$ V_{\text{média}} = \frac{39V}{2} $$

$$ V_{\text{média}} = 19,5V $$

Portanto, a tensão média entre 19,3V e 19,7V é de aproximadamente 19,5V.
##
### Correntes:
##
### Capacitância:


### Circuito FALSTAD

O circuito a seguir ilustra um esquema simplificado da Fonte de Tensão Ajustável projetada no falstad.

![Circuito fonte de tensao](https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/a9bb88d5-aff1-49af-bc49-cd9261177960)

[Link do Circuito](https://tinyurl.com/24obwzt2)

### Circuito PCB no EAGLE

#### Esquemático no EAGLE

<img width="750" alt="EAGLE" src="https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/ac880d5f-2a76-4c06-a4d0-f1967f057047">

#### Board no EAGLE

<img width="750" alt="Captura de tela 2024-06-12 211634" src="https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/608f7f37-48ac-4ff8-a1dd-6e02533ff465">

## Fotos do Projeto

![min](https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/e0ab747d-6cb8-43f0-be28-b8d9621ee088)
![max](https://github.com/JhonatanBarboza/Fonte_de_tensao/assets/170869780/7d4522fb-9ad1-4026-95a0-f721d461094a)


### Resposáveis
- Jhonatan Barboza da Silva
- João Gabriel Pieroli da Silva
- Pedro Henrique de Sousa Prestes
- Kevin Ryoji Nakashima

fonte: 

[Imagem 1](https://professor.pucgoias.edu.br/SiteDocente/admin/arquivosUpload/17742/material/Cap%204_ret%20onda%20completa_2017.pdf)

[Imagem 2](https://embarcados.com.br/aprenda-a-analisar-o-ripple-da-sua-fonte/)

