# Problemas de usabilidade recorrentes

Consolidado de 20 reuniões e de duas rodadas de suporte: 8 relatórios semanais (29/06 a 17/08/2026, ~15.700 tickets) e uma consulta direta ao HubSpot (17/08 a 17/09/2026, 9.661 tickets).

**Como ler a frequência:** número de fontes distintas que apontam o mesmo problema — cada reunião conta como uma fonte, cada semana de relatório conta como uma, e a consulta de setembro conta como **uma** fonte (foi um único recorte de 4,4 semanas, não uma leitura semana a semana). Frequência alta significa recorrência confirmada, não gravidade automática.

**Origem:** `Reuniões` (só observado em conversa), `Suporte` (só visível no volume de tickets), `Ambos` (confirmado nos dois — o sinal mais forte).

---

## Críticos — confirmados em 7+ fontes

| # | Problema | Freq | Origem | Superfície |
|---|---|---|---|---|
| 1 | Cadastro e configuração pouco intuitivos (campo de CNPJ/CPF ausente, numeração de comanda confusa, configuração difícil de achar) | 9 | Ambos | Gestor |
| 2 | Tela esconde informação que o usuário tinha um instante antes (consumo da comanda some ao lançar pagamento; pedido some ao finalizar) | 8 | Ambos | Caixa / Tablet |
| 3 | Impressora para de imprimir sem intervenção do usuário — maior falha isolada do sistema, presente em todas as 8 semanas (180 a 220 tickets/semana) e mantida em setembro (~212/semana) | 9 | Suporte | Impressão |
| 4 | Renovação de certificado digital depende 100% do suporte — fluxo manual por e-mail, sem autoatendimento | 8 | Suporte | Emissão Fiscal |
| 5 | Erro fiscal exibido em linguagem técnica crua do SEFAZ, sem ação corretiva clara | 8 | Suporte | Emissão Fiscal |
| 6 | Funcionalidade que já existe não é encontrada — maior categoria de chamados do painel inteiro, e **em crescimento**: passou de ~250 para ~379 tickets/semana em setembro | 9 | Suporte | Toda a operação |
| 7 | Divergência recorrente no fechamento de caixa (conferência, relatórios, duplicidade com iFood) | 8 | Ambos | Caixa |
| 8 | Cálculo de taxas saindo diferente do configurado (frete por raio, taxa de serviço, cobrança de módulo não usado) | 7 | Ambos | Delivery / Financeiro |
| 9 | Produto cadastrado e disponível não aparece onde deveria — no cardápio para o cliente **e no KDS para a cozinha** | 8 | Suporte | Cardápio / KDS |
| 10 | Instalar ou reconfigurar impressora não é autosserviço | 7 | Suporte | Impressão |

## Relevantes — 3 a 6 fontes

| # | Problema | Freq | Origem | Superfície |
|---|---|---|---|---|
| 11 | Mensagens automáticas de WhatsApp param de disparar (confirmação de pedido, aviso ao motoboy, relatório de fechamento) — volume crescente ao longo das semanas | 6 | Suporte | Delivery / Caixa |
| 12 | Comanda some ou trava mesmo já finalizada — risco real de perda de pedido em andamento | 5 | Suporte | Comandas |
| 13 | Operação fragmentada entre telas e sistemas — dor central mais citada nas reuniões | 4 | Reuniões | Gestor |
| 14 | Transferir item ou mesa entre comandas é difícil | 4 | Suporte | Comandas |
| 15 | Travamento e lentidão em horário de pico, com o sistema caindo várias vezes no mesmo turno | 4 | Ambos | Toda a operação |
| 16 | Mudança ou corte de funcionalidade sem comunicado prévio | 3 | Ambos | Toda a operação |
| 17 | Integração de parceiro não escala para multi-loja; configuração se perde após atualização | 3 | Ambos | Multilojas |
| 18 | Edição avançada de cardápio (complementos, duplicar item, renomear) não é encontrada | 3 | Suporte | Cardápio |
| 19 | Observação do cliente deixou de aparecer no KDS após atualização de interface — a cozinha não vê "sem cebolinha" e produz errado. Relatado por lojas diferentes no mesmo período, o que sugere regressão, não configuração | 3 | Suporte | KDS |
| 20 | Configuração do KDS não é descoberta — como criar, qual link acessar, como fazer o delivery aparecer nele | 3 | Suporte | KDS |
| 21 | Saldo do Clube/cashback se comporta de forma inesperada — não abate no pedido, aparece zerado para cliente cadastrado, expira antes do informado | 3 | Ambos | Clube |

## Emergentes — 1 a 2 fontes

| # | Problema | Freq | Origem | Superfície |
|---|---|---|---|---|
| 22 | Sem modo offline — dependência total de internet | 2 | Reuniões | Toda a operação |
| 23 | Fluxo pouco claro induz erro humano no lançamento de pagamento | 2 | Reuniões | Caixa |
| 24 | KDS não rola a página quando acumula muitos pedidos — falha justamente no pico | 1 | Suporte | KDS |
| 25 | Cashback zera o saldo inteiro em vez de descontar apenas o valor usado (mecânica específica relatada em reunião; os tickets de suporte mostram problemas de saldo, mas não confirmam esta mecânica exata — ver item 21) | 1 | Reuniões | Clube |
| 26 | Comunicação incorreta no onboarding gera expectativa não cumprida | 1 | Reuniões | Comercial → Produto |
| 27 | Nomes de pagamento parecidos confundem (Pix online vs. Pix em conta) | 1 | Reuniões | Link de pagamento |

---

## Padrões transversais

Três leituras que atravessam a lista e valem mais que qualquer item isolado:

**1. Descoberta é o maior problema do produto, não funcionalidade faltando.**
Os itens 1, 6, 9, 10, 18 e 20 são todos variações de "existe, mas não é encontrado". Somados, representam o maior bloco de chamados do painel — e o bloco está crescendo: a categoria "situação não listada" subiu de cerca de 250 para cerca de 379 tickets por semana entre agosto e setembro. Antes de aprovar construção de algo novo, verifique se o problema real é de descoberta.

**2. Dinheiro é onde o erro custa confiança, não só tempo.**
Itens 2, 7, 8, 21, 23 e 25 tocam caixa, taxas e saldo de cashback. É a categoria que gera o desgaste mais rápido e as ameaças explícitas de troca de fornecedor. Erro visual em tela de cardápio irrita; erro de R$ 5 no fechamento faz o cliente perder a confiança no sistema inteiro.

**3. O que some assusta mais que o que nunca apareceu.**
Itens 2, 12, 17 e 19 têm a mesma forma: algo que estava lá desaparece. Comanda que some, configuração que se perde, consumo que evapora ao cobrar, observação do cliente que some do KDS depois de uma atualização. Esse tipo de falha produz uma reação desproporcional ao impacto real, porque destrói a premissa de que o sistema é um registro confiável.

**4. A cozinha tem dois caminhos, e os dois falham de formas diferentes.**
Comanda impressa e KDS são rotas alternativas até a produção. A impressão falha por infraestrutura (item 3, o maior volume isolado do painel); o KDS falha por interface e configuração (itens 9, 19, 20, 24). Ao avaliar qualquer incidente de "a cozinha não recebeu o pedido", identifique primeiro qual das duas rotas a operação usa — o diagnóstico e a correção são completamente diferentes.

---

## Nota metodológica

Alguns itens de alto volume no suporte são falha técnica, não usabilidade — a impressora que para (item 3) e a queda de WhatsApp (item 11) são instabilidade de integração ou hardware. Estão aqui porque, do ponto de vista do usuário, a distinção não existe: o sistema falhou. Mas a solução para eles é de engenharia, não de design de interface. Ao priorizar, separe os dois grupos.
