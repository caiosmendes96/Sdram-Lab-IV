# Sdram-Lab-IV

O mestre Avalon lê os valores das chaves SW, escreve-os na SDRAM em um endereço fixo específico e, em seguida, esse endereço é lido e o valor é escrito nos LEDs.
## 

Input: 
  SW[7:0]

Output: LEDS[7:0]

##

<b>Como simular no Modelsim:</b>

Modificar o arquivo simulacao.do e adicionar o diretorio raiz da sua máquina:
  - set QSYS_SIMDIR <seu_diretorio>
  - Modificar essas quatros linhas do diretorio para o caminho raiz da sua máquina:

vlog C:/Users/caios/Documents/laboratorio_integrado_IV/teste/TesteTB.v para vlog <seu_diretorio>

vlog C:/Users/caios/Documents/laboratorio_integrado_IV/teste/Master_Interface.v para vlog <seu_diretorio>

vlog C:/Users/caios/Documents/laboratorio_integrado_IV/teste/TesteBdf.v para vlog <seu_diretorio>

vcom C:/Users/caios/Documents/laboratorio_integrado_IV/teste/pll.vhd para vcom <seu_diretorio>

##
<b>Após realizar essas mudanças, basta executar o macro no Modelsim a seguir:</b>

  - msim_setup.tcl
  - simulacao.do 
