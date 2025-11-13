# Sistema de Inventário em Haskell – RA2  
Pontifícia Universidade Católica do Paraná – PUCPR  
Curso: **Ciência da Computação**  
Disciplina: **Programação Funcional**  
Professor: **Frank Coelho de Alcantara**

---

## Integrantes do Grupo 

| Nome | GitHub |
|------|--------|
| Gabriel Baú | https://github.com/ogabrielbau |

---

## Link para Execução Online
GDB Online: ---------

# 1. Objetivo do Projeto

Este trabalho implementa um **sistema de gerenciamento de inventário** em Haskell, utilizando:

- Programação funcional e tipos algébricos  
- Separação total entre lógica pura e efeitos colaterais (IO)  
- Persistência de dados em arquivos (`Inventario.dat`)  
- Auditoria completa com log (`Auditoria.log`) em modo append-only  
- Execução interativa via terminal  
- Relatórios completos com análise de logs  

---

#2. Descrição Geral

O sistema permite:

- **Adicionar itens**  
- **Remover itens**  
- **Atualizar quantidade de itens**
- **Listar inventário**
- **Gerar relatório completo (report)**

Cada operação, incluindo falhas, é registrada no log.

O estado atual do inventário **persiste entre execuções**, pois é salvo em arquivo.

---

# 3. Estrutura do Projeto

