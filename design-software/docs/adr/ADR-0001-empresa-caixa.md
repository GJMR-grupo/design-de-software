# ADR-0001: Melhorar a consulta de saldo

## Status
Proposto

## Contexto

A CaixaDigital é uma empresa fictícia criada para esta atividade. O sistema apresenta lentidão quando muitas pessoas acessam o aplicativo ao mesmo tempo para consultar o saldo da conta.

## Decisão

Decidimos guardar temporariamente as consultas de saldo para que o sistema não precise buscar a mesma informação no banco de dados toda hora. Assim, as consultas ficam mais rápidas.

## Alternativas Consideradas

- Buscar o saldo diretamente no banco de dados em todas as consultas: não foi escolhida porque pode deixar o sistema mais lento quando muitas pessoas acessam ao mesmo tempo.
- Melhorar apenas o servidor: não foi escolhida porque aumentaria o custo e não resolveria o problema sozinho.

## Consequências

- O usuário consegue consultar o saldo mais rapidamente.
- O banco de dados recebe menos consultas repetidas.
- Será preciso atualizar as informações quando o saldo da conta mudar.

---

*Autor(es): Caio Gabriel, Guilherme Felipe, Michelly Lima, Júllya Andrade e Ryan Rodrigues*

*Data: 31/07/2026*
