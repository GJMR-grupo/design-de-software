# ADR-0001: Uso de cache para consultas de saldo

## Status
Proposto

## Contexto

A CaixaDigital é uma instituição financeira fictícia que atende muitos clientes diariamente. Em horários de pico, muitas pessoas acessam o aplicativo ao mesmo tempo para consultar o saldo da conta, o que gera muitas consultas ao banco de dados e deixa o sistema mais lento.

## Decisão

Vamos utilizar um sistema de cache para armazenar temporariamente as consultas de saldo. Dessa forma, consultas repetidas poderão ser respondidas rapidamente, reduzindo o peso no banco de dados.

## Alternativas Consideradas

- Consultar o banco de dados em todas as requisições: descartada porque aumenta o tempo de resposta e sobrecarrega o banco.
- Aumentar apenas a capacidade do servidor: descartada porque aumenta os custos e não resolve o problema de forma eficiente.

## Consequências

- As consultas de saldo serão mais rápidas para o usuário.
- O banco de dados receberá menos acessos repetitivos.
- Será necessário manter o cache atualizado sempre que houver movimentação na conta, para evitar informações desatualizadas.

---

*Autor(es): Caio Gabriel, Guilherme Felipe, Michelly Lima, Júllya Andrade e Ryan Rodrigues*

*Data: 31/07/2026*
