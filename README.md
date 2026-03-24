# Desafio Bancário - Aplicação Console em Java

## Sistema bancário simples desenvolvido em Java para execução via terminal.
Implementa operações básicas de consulta de saldo, transferência via Pix e recebimento de valores através de um menu interativo.

## Funcionalidades
- Consulta de saldo atual da conta
- Realização de Pix com validação de saldo suficiente
- Recebimento de valores para acréscimo no saldo
- Encerramento seguro do programa

## Requisitos
- Java JDK 17 ou superior (suporte a Text Blocks requerido)

## Instruções de Execução

### Compilação e Execução
```bash
# Compilar o código fonte 
javac Desafio.java  
# Executar a aplicação 
java Desafio 
```

### Plataformas Suportadas
- Linux / macOS / Windows (com Java instalado)

## Exemplo de Uso
```plaintext
**************************
Nome do cliente: Jota  
Tipo Conta: Corrente  
Saldo atual: 1500.0  
***************************
**Digite sua opção**
1 - Consultar saldo  
2 - Fazer pix  
3 - Receber valor  
4 - Sair  
---------------------
> 2  
Qual o valor do pix:  > 500  
Saldo atual: 1000.0   
```

## Estrutura do Projeto
```plaintext
desafio-bancario/  
└── Desafio.java           # Classe principal com lógica completa   
```

## Tecnologias Utilizadas
| Tecnologia | Finalidade |
|--------------|------------|
java 17+ | Linguagem de programação principal |
java.util.Scanner | Leitura de entrada do usuário |
'text Blocks' | Formatação de menus (Java 15+) |

## Limitações do Sistema Atual
- Dados do cliente fixos no código fonte.
- Ausência de persistência de dados (memória volátil).
- Validação limitada de entrada do usuário.
- Bug na opção de saída (exibe mensagem de opção inválida).

## Plano de Evolução
1. Implementação de persistência com arquivos JSON.
2. Suporte a múltiplas contas de usuário.
3. Validação robusta de entradas numéricas.
4. Sistema de extrato de transações.
5. Correção do fluxo de saída do programa.
6. Suporte a diferentes tipos de conta.
7. Histórico de operações com timestamp.

## Observações Técnicas
- O programa utiliza loop `while` para menu interativo.
- Validação de saldo implementada antes do Pix.
- Text Blocks utilizados para formatação limpa do menu.
e - Encerramento via `System.exit(0)` na opção 4.

## Autor
**João Victor**
