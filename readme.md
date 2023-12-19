# Processador MIPS Simples
Este projeto consiste em um processador básico baseado na arquitetura MIPS (Microprocessor without Interlocked Pipeline Stages) implementado em VHDL. O processador suporta apenas parte do conjunto de instruções MIPS para realizar operações simples.  
A arquitetura completa do processador pode ser visualizada na figura abaixo:  
![Arquitetura do Processador](MIPS.pdf)

Instruções Suportadas
O processador suporta as seguintes instruções:

**LW** - Carrega um valor da memória para um registrador.  
**SW** - Armazena o valor de um registrador na memória.  
**ADD** - Soma dois registradores e armazena o resultado em um terceiro registrador.  
**SUB** - Subtrai o conteúdo de um registrador do conteúdo de outro registrador e armazena o resultado em um terceiro registrador.  
**AND** - Realiza a operação lógica AND bit a bit entre dois registradores e armazena o resultado em um terceiro registrador.  
**OR** - Realiza a operação lógica OR bit a bit entre dois registradores e armazena o resultado em um terceiro registrador.  
**NOR** - Realiza a operação lógica NOR bit a bit entre dois registradores e armazena o resultado em um terceiro registrador.  
**SLT** - Define um registrador como 1 se o valor de um registrador for estritamente menor que o valor de outro registrador, caso contrário, define como 0.  
**SLTI** - Define um registrador como 1 se o valor de um registrador for estritamente menor que um valor imediato, caso contrário, define como 0.  
**BEQ** - Desvia a execução do programa para um endereço específico se dois registradores forem iguais.  
**J** - Desvia a execução do programa para um endereço específico.  
**JAL** - Desvia a execução do programa para um endereço específico e salva o endereço de retorno no registrador $ra.  
**JR** - Desvia a execução do programa para um endereço específico armazenado em um registrador.  
**BNE** - Desvia a execução do programa para um endereço específico se dois registradores forem diferentes.  
**NOP** - Não faz nada.  
**ADDI** - Soma um valor imediato a um registrador e armazena o resultado em um terceiro registrador.  
**ORI** - Realiza a operação lógica OR bit a bit entre um registrador e um valor imediato e armazena o resultado em um terceiro registrador.  
**LUI** - Carrega um valor imediato de 16 bits para os 16 bits mais significativos de um registrador.  
**SLL** - Desloca o conteúdo de um registrador para a esquerda e armazena o resultado em um terceiro registrador.  
**SRL** - Desloca o conteúdo de um registrador para a direita e armazena o resultado em um terceiro registrador.  
**LBU** - Carrega um byte da memória para um registrador.  

## Como Utilizar
Clone o Repositório  
Compile os arquivos VHDL  
Execute a simulação para observar o comportamento do processador ou teste gravando na sua FPGA  

O arquivo de teste em ROMContent.mif contém o código em assembly que será executado pelo processador. É um código básico que testa algumas instruções do processador e pode ser alterado para testar outras instruções.

## Contribuições
Contribuições são bem-vindas! Se encontrar algum problema ou tiver melhorias a sugerir, sinta-se à vontade para abrir uma issue ou enviar um pull request.

# Simple MIPS Processor
This project is a basic processor based on the MIPS (Microprocessor without Interlocked Pipeline Stages) architecture implemented in VHDL. The processor only supports a subset of the MIPS instruction set to perform simple operations.

The complete architecture of the processor can be seen in the figure above

## Supported Instructions
The processor supports the following instructions:

**LW** - Loads a value from memory into a register.  
**SW** - Stores the value of a register in memory.  
**ADD** - Adds two registers and stores the result in a third register.  
**SUB** - Subtracts the contents of one register from the contents of another register and stores the result in a third register.  
**AND** - Performs the bitwise AND logical operation between two registers and stores the result in a third register.  
**OR** - Performs the bitwise OR logical operation between two registers and stores the result in a third register.  
**NOR** - Performs the bitwise NOR logical operation between two registers and stores the result in a third register.  
**SLT** - Sets a register to 1 if the value of one register is strictly less than the value of another register, otherwise sets it to 0.  
**SLTI** - Sets a register to 1 if the value of a register is strictly less than an immediate value, otherwise sets it to 0.  
**BEQ** - Branches the program execution to a specific address if two registers are equal.  
**J** - Branches the program execution to a specific address.  
**JAL** - Branches the program execution to a specific address and saves the return address in the $ra register.  
**JR** - Branches the program execution to a specific address stored in a register.  
**BNE** - Branches the program execution to a specific address if two registers are different.  
**NOP** - Does nothing.  
**ADDI** - Adds an immediate value to a register and stores the result in a third register.  
**ORI** - Performs the bitwise OR logical operation between a register and an immediate value and stores the result in a third register.  
**LUI** - Loads a 16-bit immediate value into the 16 most significant bits of a register.  
**SLL** - Shifts the contents of a register to the left and stores the result in a third register.  
**SRL** - Shifts the contents of a register to the right and stores the result in a third register.  
**LBU** - Loads a byte from memory into a register.  

## How to Use
Clone the repository
Compile the VHDL files
Run the simulation to observe the processor behavior or test by writing to your FPGA
The test file in ROMContent.mif contains the assembly code that will be executed by the processor. It is a basic code that tests some of the processor's instructions and can be modified to test other instructions.

## Contributing
Contributions are welcome! If you find any issues or have improvements to suggest, feel free to open an issue or submit a pull request.