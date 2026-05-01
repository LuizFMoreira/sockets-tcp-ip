# Programação em Sockets TCP/IP

Implementação e testes de programação em sockets utilizando os protocolos UDP, TCP e TCP Concorrente (Multithread).

---

**Aluno:** LUIZ FERNANDO BATISTA MOREIRA  
**Curso:** Engenharia de Software  
**Disciplina:** Redes de Computadores 
**Professor:** Marco Aurelio de Souza Birchal  
**Data:** Abril de 2026

---

## 📋 Conteúdo

- **UDPServer.py** – Servidor UDP que converte mensagens para maiúsculas
- **UDPClient.py** – Cliente UDP que envia mensagens e recebe respostas
- **TCPServer.py** – Servidor TCP sequencial (um cliente por vez)
- **TCPClient.py** – Cliente TCP que se conecta ao servidor
- **TCPConcurrentServer.py** – Servidor TCP com múltiplas threads (atende vários clientes)
- **TCPConcurrentClient.py** – Cliente TCP que se conecta ao servidor concorrente
- **Relatorio_Sockets.docx** – Relatório completo com código, execução e explicações

## 🚀 Como Executar

### UDP

**Terminal 1 (Servidor):**
```bash
py UDPServer.py
```

**Terminal 2 (Cliente):**
```bash
py UDPClient.py
```
Digite uma frase em minúsculas e pressione Enter. O servidor retorna em maiúsculas.

### TCP

**Terminal 1 (Servidor):**
```bash
py TCPServer.py
```

**Terminal 2 (Cliente):**
```bash
py TCPClient.py
```
Digite uma frase e pressione Enter. O servidor retorna em maiúsculas.

### TCP Concorrente

**Terminal 1 (Servidor):**
```bash
py TCPConcurrentServer.py
```

**Terminal 2 (Cliente 1):**
```bash
py TCPConcurrentClient.py
```

**Terminal 3 (Cliente 2):**
```bash
py TCPConcurrentClient.py
```

Digite mensagens em cada cliente. Pressione CTRL+X para sair.
O servidor suporta múltiplos clientes simultâneos através de threads.

## 📝 Características

| Protocolo | Conexão | Confiabilidade | Múltiplos Clientes | Porta |
|-----------|---------|----------------|-------------------|-------|
| UDP | Não | Não garantida | Sim (sem estado) | 12000 |
| TCP | Sim | Garantida | Não (sequencial) | 12000 |
| TCP Concorrente | Sim | Garantida | Sim (threads) | 50000 |

## 📖 Referência

Baseado no slide: **REDES3_ES_TCP_Sockets_Parte2.pdf**

Disciplina: Redes de Computadores 3
