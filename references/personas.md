# Personas e comportamento

Quatro personas extraídas de 20 reuniões (comercial, onboarding e sucesso) e cruzadas com 8 semanas de tickets de suporte. Nomes fictícios. Nenhuma sessão é atribuída a um membro específico do time Takeat.

**Confiança:** Hipótese (1 fonte) < Emergente (2–4 fontes) < Validada (5+ fontes convergentes).

**Índice**
- [Renata — a dona que resolve tudo](#renata)
- [Bruno — o operador que não decide a compra](#bruno)
- [Cristina — a gestora de rede](#cristina)
- [Eduardo — o potencial cliente em decisão](#eduardo)
- [Comensal — hipótese, não persona](#comensal)
- [Comportamento do time Takeat](#time-takeat)
- [Contexto ambiental observado](#contexto-ambiental)

---

<a id="renata"></a>
## Renata — a dona que resolve tudo

**Camada:** Decisora + Operadora · **Confiança:** Validada · **Fontes:** 12

O padrão mais recorrente de todos. Aparece em mais da metade das reuniões analisadas.

**Perfil de negócio.** Restaurante, bar, hamburgueria ou lanchonete independente. Uma unidade — às vezes ainda nem abriu. Equipe enxuta. Ela acumula caixa, financeiro, cardápio, atendimento e configuração do sistema. Decide sozinha ou com o cônjuge/sócio.

**Job to be done.** Ter a operação inteira numa tela só, sem depender de planilha paralela nem de terceiros. A régua de sucesso é simples: no fim do dia, o que o sistema diz que faturou tem que bater com o que entrou no caixa.

**Rotina no sistema.** Abertura e fechamento de caixa, emissão de nota, configuração de cardápio e delivery, conferência de pedidos, atendimento ao cliente final quando precisa.

**Dores (em ordem de intensidade observada):**
1. Divergência no fechamento de caixa — a que mais gera desgaste
2. Fluxo fragmentado entre telas e sistemas
3. Tela esconde informação que ela tinha um segundo antes (consumo da comanda, status do pedido)
4. Travamento e lentidão no horário de pico, justamente quando não pode parar
5. Cadastro sem campos essenciais (CNPJ/CPF do cliente PJ)
6. Mudança no sistema sem aviso prévio
7. Dependência total de internet, sem modo offline

**Comportamento observado:**
- Admite estar perdida e se culpa antes de culpar a interface, mesmo se descrevendo como capaz de aprender rápido.
- Mantém planilha paralela mesmo pagando pelo sistema — não é desconhecimento, é rede de segurança e um sinal de desconfiança raramente verbalizado como reclamação.
- Cria gambiarra (desabilita opção, usa refresh, evita fluxo que sabe que trava) antes de reclamar formalmente — por isso o volume de chamados de suporte subestima o problema real.
- Aciona o suporte antes de procurar o caminho sozinha: "situação não listada" é a maior categoria do painel em todas as 8 semanas analisadas (200 a 307 tickets/semana), quase toda sobre funcionalidade que já existe.
- Separa a qualidade do produto da qualidade do atendimento — diz que gosta do sistema e que está desgastada com ele na mesma frase. É um cliente que ficaria se o básico funcionasse.
- A ameaça de churn é silenciosa: não é o problema isolado que faz sair, é o desgaste por repetição sem resolução — e só revela que cogitava trocar de fornecedor depois que o problema já foi resolvido.

**Necessidades não atendidas.** Modo offline; campos de cadastro completos; aviso antecipado de mudanças; estabilidade no pico.

**O que ela disse:**
> "Eu tenho tudo numa tela só. Lá fica tudo fragmentado."

> "Eu estou literalmente perdida mesmo, tá? [...] eu tenho muita facilidade pra aprender."

> "Quando eu abro a comanda, o consumo desaparece."

> "O que mais importa pra mim é fechamento geral, né? Lá, falou que vendeu três mil e fechou três mil, aí o caixa bateu."

> "Todo dia a mesma coisa, a mesma coisa, e a gente fala e não resolve, fala, não resolve, e vai desgastando."

> "O resto do sistema é muito bom, gosto mais dele, do jeito de trabalhar dele, mas fica essa situação, entendeu? Falhando o tempo inteiro."

**Ao projetar para Renata:** ela não tem tempo de aprender. Qualquer passo a mais no fechamento de caixa é um passo que ela vai fazer 365 vezes por ano, sob pressão, no fim de um turno cansativo.

---

<a id="bruno"></a>
## Bruno — o operador que não decide a compra

**Camada:** Operador (não decisor) · **Confiança:** Emergente · **Fontes:** 4

Hipótese bem sustentada, mas ainda não validada. Precisa de mais fontes.

**Perfil.** Funcionário, sócio júnior ou parceiro terceirizado (contador, consultor financeiro) responsável por uma função específica: fechamento de caixa, configuração de delivery, parte fiscal. Não escolheu o sistema — herdou junto com a função.

**Job to be done.** Executar sua tarefa sem errar e sem precisar escalar toda hora para o dono.

**Rotina no sistema.** Fechamento e conferência de caixa, configuração pontual de um módulo, repasse de dúvidas para quem decide. Usa poucas telas, com profundidade.

**Dores.** Não recebeu acesso nem treinamento a tempo. Se perde nas telas que usa com pouca frequência. Precisa adivinhar onde fica cada configuração. O onboarding foi desenhado pensando no decisor, não nele.

**Comportamento observado:**
- Admite abertamente quando não sabe algo, sem rodeio, e documenta bem quando pedido (print, vídeo).
- Vai bem com passo a passo acompanhado em tempo real, mas trava sozinho — sucesso durante a call não prevê sucesso depois dela.
- Prefere pedir acesso remoto ao suporte a seguir um tutorial, visível nos tickets de impressora e cardápio (pedidos explícitos de TeamViewer/AnyDesk) — o custo percebido de aprender o fluxo é maior que o custo de esperar o suporte.

**Necessidades não atendidas.** Onboarding por perfil de usuário, não por conta. Configurações mais visíveis e autoexplicativas.

**O que ele disse:**
> "Eu não sei o que estava acontecendo."

> "Eu não peguei nada [os acessos ao sistema], eu não estou a..."

**Ao projetar para Bruno:** ele é o teste mais duro de descoberta. Se a funcionalidade só é encontrável por quem já sabe onde ela fica, ela não existe para ele.

---

<a id="cristina"></a>
## Cristina — a gestora de rede

**Camada:** Decisora + Coordenadora de múltiplas unidades · **Confiança:** Emergente · **Fontes:** 4

**Perfil.** Responde por várias lojas, marcas ou quiosques ao mesmo tempo. Centraliza suporte, configuração e treinamento da rede inteira. Decisão às vezes compartilhada com sócios ou franqueados.

**Job to be done.** Visão consolidada entre unidades (DRE, estoque, configuração) com padronização — e previsibilidade sobre o que vai mudar no sistema.

**Rotina no sistema.** Corrige configuração fiscal e financeira de todas as lojas, faz ponte entre as lojas e a Takeat, coordena treinamentos internos.

**Dores.** Integração de parceiro que não escala para multi-loja (ex: canal de delivery que só sincroniza com uma unidade). Perda de configuração após atualização, afetando várias lojas de uma vez. Mudança de tela sem aviso prévio gerando onda simultânea de dúvidas. Ausência de log de auditoria para rastrear quem alterou o quê.

**Comportamento observado:**
- Cobra aviso prévio antes de qualquer mudança de tela — uma alteração não avisada vira onda simultânea de dúvidas em toda a rede, porque o custo dela é multiplicado pelo número de lojas.
- Já cogitou migrar de sistema quando os problemas se acumularam, e reverteu ao sentir que estava sendo ouvida de verdade — atenção direta recupera confiança mais rápido do que o histórico de problemas sugeriria.
- Vira multiplicadora interna quando confia no sistema: passou a corrigir a configuração de todas as lojas por conta própria, convertendo confiança conquistada em trabalho que a Takeat não precisa fazer.

**Necessidades não atendidas.** Comunicação antecipada de mudanças; log de auditoria; treinamento segmentado por perfil (líder de loja vs. franqueado).

**O que ela disse:**
> "São sete lojas que ficam atrás de mim [...] fala que é erro, mas é erro que apareceu do nada."

> "Eu já estava olhando outro sistema pra migrar [...] mas agora parece que deu certo, fico muito feliz."

> "Seria mais prático ter essa antecipação. Primeiro mostra o que serão as alterações, depois a gente atualiza."

**Ao projetar para Cristina:** o custo de um erro é multiplicado pelo número de lojas. Ela é a persona em que "avisar antes" vale mais que "resolver rápido depois".

---

<a id="eduardo"></a>
## Eduardo — o potencial cliente em decisão

**Camada:** Potencial cliente (decisor, ainda não é cliente) · **Confiança:** Validada como padrão de compra · **Fontes:** 8

**Perfil.** Dono de negócio novo (às vezes ainda não abriu) ou insatisfeito com o sistema atual. Está comparando fornecedores ativamente, com 2 a 3 apresentações agendadas.

**Job to be done.** Escolher o sistema certo sem pagar por complexidade que não vai usar, e sem repetir a dor que já viveu com o fornecedor anterior.

**Rotina na decisão.** Agenda demonstrações de concorrentes, pergunta preço, taxas adicionais, multa de cancelamento e disponibilidade de suporte.

**Dores e gatilhos.** Trauma com suporte ausente num momento crítico. Custo alto do sistema atual. Ausência de uma funcionalidade que considera decisiva. Operação espalhada em vários aplicativos.

**Concorrentes citados espontaneamente nas reuniões:** Zig, Anota AI, Saipos. Os motivos de insatisfação mais citados com o fornecedor anterior são custo alto, suporte ausente em momento crítico e relatórios de pós-venda insuficientes — os três aparecem quase sempre juntos, não isolados.

**Comportamento observado:**
- É transparente sobre estar comparando fornecedores — cita quantas apresentações já viu e vai ver, sem esconder do vendedor.
- O trauma com o fornecedor anterior molda o que ele pergunta: quem ficou sem suporte numa data crítica pergunta insistentemente sobre disponibilidade de atendimento — a pergunta revela a cicatriz, não só o requisito.
- Testa o vendedor com perguntas objetivas de custo e cancelamento.
- Raramente decide sozinho, mesmo sendo o contato principal: quase sempre precisa validar com sócio ou cônjuge ausente da reunião.

**Necessidades não atendidas.** Clareza total do custo (módulos adicionais, CNPJ extra). Prova concreta de que o suporte responde em momento crítico.

**O que ele disse:**
> "Vocês são as primeiras pessoas que eu converso. Então eu não tenho embasamento nenhum."

> "A gente já teve duas empresas, aí tem a sua agora, vamos ter outra amanhã, a gente vai ponderar quem está mais ou menos."

> "O problema do sistema anterior são dois: o custo é bem caro, e os relatórios de pós-venda deixam a desejar."

**Ao projetar para Eduardo:** o material de venda dele compete com a memória do fornecedor anterior. Promessa não cumprida no onboarding vira dor de cliente no mês seguinte — há evidência de funcionalidade anunciada como inclusa que não estava disponível.

---

<a id="comensal"></a>
## Comensal — hipótese, não persona

O cliente final do restaurante aparece em várias reuniões, mas **sempre relatado pelo operador, nunca observado diretamente**. Não foi promovido a persona por isso.

Comportamento relatado:
- Confunde opções de pagamento com nomes parecidos no mesmo link (Pix online vs. Pix em conta)
- Quer visibilidade do status do pedido sem precisar perguntar a alguém — depois de finalizar no tablet, o pedido some da tela
- Abandona o pedido quando o cardápio de delivery está confuso ou com operações diferentes misturadas

**Para virar persona validada**, precisa de entrevista direta com consumidor final. Até lá, qualquer decisão apoiada só nesses sinais deve vir com recomendação de validação.

---

<a id="time-takeat"></a>
## Comportamento do time Takeat

Como quem atende se comporta nas reuniões, porque isso molda o que o cliente relata e afeta a leitura de toda a evidência acima:

- Quando não sabe algo, o padrão é prometer verificar e voltar depois — saudável, mas deixa muita informação pendente de retorno assíncrono. Repete em pelo menos 4 reuniões: bug intermitente, prazo de correção, funcionalidade indisponível, integração de parceiro.
- Corrige erro de configuração ao vivo, de forma reativa (ex: CNPJ vinculado errado, número de sabores de pizza incorreto) — sinal de que não há verificação proativa pós-setup.
- Já comunicou informação incorreta em venda ou onboarding pelo menos uma vez identificada (funcionalidade anunciada como inclusa que não estava disponível), gerando expectativa furada que aparece como frustração semanas depois.
- Só propõe solução estrutural depois que o problema se repete várias vezes — ex: log de auditoria só foi proposto após relatos repetidos de perda de configuração. A primeira ocorrência tende a virar atendimento pontual, não sinal.
- Há registro de solicitação de cliente aberta há cerca de um ano e meio, ainda sem solução nem retorno, alimentando diretamente a percepção de abandono.

---

<a id="contexto-ambiental"></a>
## Contexto ambiental observado

Não é comportamento de uma pessoa específica, mas condições recorrentes do ambiente onde a operação acontece — moldam por que os comportamentos acima existem, e valem para quem for desenhar qualquer fluxo:

- **O pico de movimento é o momento em que quase todos os problemas críticos aparecem**, e é exatamente quando ninguém tem tempo de investigar nada. Qualquer fluxo de recuperação de erro precisa funcionar sob pressão, não só em teste tranquilo.
- **Boa parte das operações roda em computador ou celular compartilhado, com o WhatsApp aberto ao lado** — a atenção é dividida por padrão, não por distração pontual.
- **A internet do estabelecimento é ponto único de falha e frequentemente instável.**
- **A cozinha tem duas rotas possíveis até o pedido, e elas falham de formas diferentes.** Comanda impressa depende de infraestrutura (a impressora é a maior fonte de chamados técnicos do painel de suporte); KDS depende de interface e configuração (tela de observação que some, rolagem que trava no pico, configuração pouco descoberta). Há operações com vários KDS em sequência — linhas de produção diferentes mais uma expedição — onde a impressão só é acionada no fim do fluxo. Não assumir uma única rota nem um KDS único por loja. Ver [usabilidade.md](usabilidade.md) para o detalhamento dos problemas específicos de cada rota.
