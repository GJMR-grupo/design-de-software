# ADR-0002: Definições iniciais para o aplicativo da fila da cantina

## Status
Proposto

## Contexto

A cantina do campus costuma ficar cheia no horário de almoço, fazendo com que muitos alunos enfrentem filas demoradas ou até desistam de comprar a refeição. Para tentar melhorar essa situação, a coordenação propôs a criação de um aplicativo simples, onde o aluno possa reservar o prato do dia antes de chegar à cantina e retirar o pedido de forma mais rápida.
Durante a discussão, surgiram algumas dúvidas que ainda precisam ser definidas, como a forma de pagamento e o que fazer quando um aluno faz a reserva, mas não comparece para buscar o pedido. Além disso, como a cantina possui poucos funcionários, a solução precisa ser simples e não aumentar o trabalho da equipe.

## Decisão

### Decisão 1 – O pagamento será realizado pelo aplicativo.

Essa decisão foi tomada para reduzir o tempo de atendimento no caixa e diminuir a fila, trazendo mais praticidade para o aluno.

### Decisão 2 – A retirada do pedido será feita por meio de um QR Code.

O aluno apresenta o QR Code gerado no aplicativo e o funcionário faz a entrega do pedido. Isso torna a retirada mais rápida e evita a conferência manual dos pedidos.

### Decisão 3 – Não haverá reembolso quando o aluno reservar e não comparecer por motivo pessoal.

Essa decisão evita desperdício de alimentos e prejuízo para a cantina quando o pedido já tiver sido preparado.

## Alternativas Consideradas

- **Manter o pagamento apenas na cantina:** não foi escolhido porque o aluno ainda precisaria passar pelo caixa, o que diminuiria o benefício de retirar o pedido rapidamente e o problema de filas permaneceria.

- **Entregar o pedido informando apenas o nome ou a matrícula:** não foi escolhido porque pode causar demora na hora de conferir e aumentar a chance de erros. O QR Code torna a retirada mais rápida e segura para a cantina.

- **Permitir reembolso quando o aluno não comparecer para retirar o pedido:** não foi escolhido porque poderia aumentar o desperdício de alimentos e gerar prejuízo para a cantina.

## Consequências

- O tempo de espera dos alunos será reduzido.
- O atendimento ficará mais organizado.
- Os funcionários não precisarão realizar muitas etapas durante a entrega dos pedidos.
- Alguns alunos podem não gostar da política de não reembolso, mas ela ajuda a evitar desperdícios.
---

*Autor(es): Caio Gabriel, Guilherme Felipe, Michelly Lima, Júllya Andrade e Ryan Rodrigues*

*Data: 04/08/2026*
