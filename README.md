# Projeto 5 COBOL - Processamento de Transacoes Bancarias

Esta versao junta:
- os registros originais do enunciado;
- os exemplos de erro descritos no projeto.

Nao ha instalador neste ZIP. Os arquivos estao separados para copiar/usar no TK5.

## Estrutura

COBOL/MOVBAN.cbl
JCL/COMPMOV.jcl
JCL/EXEMOV.jcl
DATA/CLIENTES.txt
DATA/TRANSACOES.txt
SAIDA_ESPERADA/SAIDAS_ESPERADAS.txt

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

## Arquivo CLIENTES

Os clientes foram mantidos iguais ao enunciado, com espacos para fechar o nome em 30 caracteres.

## Arquivo TRANSACOES

Este arquivo junta:
1. as 3 transacoes originais do enunciado;
2. os exemplos de validacao/erro pedidos na descricao.

Assim o programa consegue demonstrar:
- credito;
- debito;
- cliente inexistente;
- tipo de transacao invalido;
- valor zerado;
- saldo insuficiente.
