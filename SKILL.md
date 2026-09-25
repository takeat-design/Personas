---
name: takeat-personas
description: "Conhecimento de pesquisa sobre quem são os clientes e usuários da Takeat (plataforma de tecnologia para restaurantes) — 4 personas validadas, padrões de comportamento e problemas de usabilidade recorrentes, extraídos de reuniões reais e de tickets de suporte. Use sempre que a tarefa envolver produto, design, UX writing, priorização, discovery, suporte ou comercial da Takeat — inclusive quando o pedido não citar 'persona' explicitamente. Gatilhos típicos — desenhar ou revisar uma tela, escrever microcopy, avaliar uma ideia de feature, priorizar backlog, escrever spec ou PRD, interpretar um ticket, decidir entre duas soluções, ou qualquer pergunta do tipo 'o usuário entenderia isso?' e 'faz sentido pro nosso cliente?'. Na dúvida sobre o usuário da Takeat, consulte esta skill antes de responder por suposição."
---

# Clientes e usuários da Takeat

A Takeat é uma plataforma brasileira de tecnologia para restaurantes: PDV/caixa, comanda e mesa, cardápio digital, delivery, totem, Garçom Digital, emissão fiscal, Área do Gestor e Multilojas.

Esta documentação existe porque decisões de produto na Takeat costumam errar por um motivo específico: **quem compra o sistema quase nunca é quem opera ele no dia a dia**, e o dono de restaurante pequeno frequentemente é as duas pessoas ao mesmo tempo. Projetar para "o restaurante" genérico produz telas que o dono aprova e o operador não consegue usar no meio do rush.

## Como usar

1. **Identifique a persona afetada** pela decisão (tabela abaixo). Se mais de uma, diga qual é a primária e qual é a secundária — elas costumam ter interesses opostos.
2. **Leia a seção relevante antes de opinar:**
   - [references/personas.md](references/personas.md) — as 4 personas completas (rotina, dores, objetivos, comportamento, citações), o comportamento do time Takeat e o contexto ambiental em que a operação acontece
   - [references/usabilidade.md](references/usabilidade.md) — problemas recorrentes já mapeados, com frequência e origem
3. **Cite a evidência** quando justificar uma recomendação: nome da persona, número de fontes, e se veio de reunião, de suporte ou dos dois.

Esta documentação cobre **quem são os clientes e como eles se comportam** — não como o produto funciona. Para nome exato de feature, comportamento atual de uma tela, ou regra de negócio (o que uma configuração faz, como um cálculo é feito), use a fonte de verdade do produto (documentação, código, ou a pessoa responsável), não este material. Vocabulário de operação de restaurante (comanda, mesa, fechamento de caixa etc.) também não está documentado aqui — é conhecimento de setor que qualquer IA já traz.

## As 4 personas

| Persona | Quem é | Camada | Confiança |
|---|---|---|---|
| **Renata** | Dona de um restaurante que acumula caixa, financeiro, cardápio e atendimento sozinha | Decisora + Operadora | Validada (12 fontes) |
| **Bruno** | Funcionário ou parceiro responsável por uma função específica; não escolheu o sistema | Operador, não decisor | Emergente (4 fontes) |
| **Cristina** | Responde por várias lojas; centraliza configuração e treinamento da rede | Decisora + Coordenadora | Emergente (4 fontes) |
| **Eduardo** | Dono comparando fornecedores agora; ainda não é cliente | Potencial cliente | Validada (8 fontes) |

O **comensal** (cliente final do restaurante) aparece nas evidências apenas de forma relatada pelo operador, nunca observado diretamente. Trate como hipótese, não como persona validada.

## Heurísticas de decisão

Use estas regras para escolher a persona primária rapidamente:

- **Mexe em caixa, fechamento ou dinheiro** → Renata é primária. A régua dela é uma só: o que o sistema diz que faturou tem que bater com o que entrou. Divergência de caixa é a dor que mais gera desgaste e ameaça de churn.
- **Mexe em configuração, cadastro ou setup** → Bruno é primária. Ele executa sem ter escolhido o sistema e sem treinamento completo. Se a tela só funciona pra quem já sabe onde clicar, ela falha com ele.
- **Mexe em algo que afeta várias lojas ao mesmo tempo** → Cristina é primária, e **comunicação antecipada não é opcional**. Mudança sem aviso prévio vira onda simultânea de chamados na rede inteira.
- **Mexe em preço, plano, contrato ou material de venda** → Eduardo é primária. Ele está comparando fornecedores agora e testa o vendedor com perguntas objetivas de custo e cancelamento.
- **Mexe em algo que o comensal vê** (cardápio, link de pagamento, status do pedido) → cuidado: a evidência é de segunda mão. Recomende validar com o consumidor final antes de decidir.

Dois princípios que atravessam todas as personas:

- **Informação que some é pior que informação ausente.** O padrão mais citado nas reuniões é a tela esconder algo que a pessoa tinha um segundo antes (o consumo da comanda ao lançar o pagamento, o pedido ao finalizar). Ao propor qualquer fluxo, verifique o que deixa de estar visível em cada passo.
- **A funcionalidade existir não significa que ela seja encontrada.** A maior categoria de chamados do suporte, em todas as semanas analisadas, é dúvida sobre recurso que já existe. Antes de propor construir algo novo, verifique em [references/usabilidade.md](references/usabilidade.md) se o problema real é de descoberta.

## Regras de integridade

Esta documentação é fruto de pesquisa, e o valor dela depende de não ser contaminada por invenção:

- **Não invente atributos de persona.** Se alguém perguntar a idade, a renda ou o traço de personalidade de uma persona, responda que a pesquisa não cobre isso. É melhor uma lacuna declarada do que um dado fabricado que depois vira decisão.
- **Respeite o nível de confiança.** Personas "Emergentes" (Bruno, Cristina) vêm de 4 fontes cada — sustentam uma hipótese, não uma conclusão. Sinalize isso ao recomendar algo que dependa só delas.
- **Não atribua evidência a pessoas reais.** Todos os nomes são fictícios e nenhuma sessão é atribuída a um membro específico do time Takeat. Mantenha assim em qualquer output.
- **Separe relatado de observado.** Comportamento do comensal foi relatado pelo operador. Isso muda o peso da evidência e deve ser dito.
- **Se a evidência não existir, diga.** Uma recomendação honesta sem lastro ("não temos dado sobre isso; sugiro validar assim") é mais útil que uma citação forçada de persona.

## Atualizando esta documentação

É documento vivo. Quando novas reuniões ou relatórios de suporte forem processados: atualize o contador de fontes e a confiança da persona afetada em `personas.md` (Hipótese → Emergente com 2–4 fontes → Validada com 5+); para usabilidade, incremente a frequência de um problema já existente ou crie um novo na faixa correspondente em `usabilidade.md`. O Notion do time é a fonte de verdade por trás dos dois arquivos.
