# Acelera Maker ex 5
# Projeto 5 COBOL - Processamento de Transacoes Bancarias

Projeto desenvolvido em COBOL para ambiente Mainframe TK5/MVS 3.8j.

## Estrutura

COBOL/MOVBAN.cbl
JCL/COMPMOV.jcl
JCL/EXEMOV.jcl
DATA/CLIENTES.txt
DATA/TRANSACOES.txt

## Data sets sugeridos no TK5

HERC01.P5COBOL(MOVBAN)  -> codigo COBOL
HERC01.P5JCL(COMPMOV)   -> JCL de compilacao
HERC01.P5JCL(EXEMOV)    -> JCL de execucao
HERC01.P5CADCLI         -> entrada de clientes, PS, FB, LRECL 44
HERC01.P5MOVTRX         -> entrada de transacoes, PS, FB, LRECL 20
HERC01.P5LOAD(MOVBAN)   -> programa compilado
HERC01.P5SALDOS         -> saida de saldos atualizados
HERC01.P5LOGERR         -> saida de erros
HERC01.P5RESBAN         -> relatorio final

Assim o programa consegue demonstrar:
- credito;
- debito;
- cliente inexistente;
- tipo de transacao invalido;
- valor zerado;
- saldo insuficiente.
