# takeat-personas

Documentação viva de pesquisa sobre os clientes e usuários da Takeat — quem são, como se comportam, e onde o produto trava para eles. Base de evidência: 20 reuniões de comercial, onboarding e sucesso, mais duas rodadas de suporte (8 relatórios semanais e uma consulta direta ao HubSpot).

## Estrutura

```
takeat-personas/
├── SKILL.md                       entrada única: instruções + heurísticas de decisão
├── README.md                      este arquivo
└── references/
    ├── personas.md                 4 personas, comportamento (incluindo o time Takeat) e contexto ambiental
    └── usabilidade.md              27 problemas recorrentes, com frequência e origem
```

Quatro arquivos, nenhum com mais de 160 linhas. `SKILL.md` é curto de propósito — ensina *como raciocinar* com as personas e aponta pros dois arquivos de `references/`, que só precisam ser abertos quando a pergunta exigir profundidade.

## Como usar

**Ferramenta com suporte a Skill** (Claude Code, Claude.ai, Cowork): coloque a pasta no diretório de skills do projeto. A IA passa a consultar sozinha quando a tarefa envolver produto, design ou atendimento da Takeat.

**Qualquer outra IA, ou leitura humana:** `SKILL.md` funciona sozinho, sem ferramenta nenhuma — abra direto no GitHub ou cole o conteúdo no início de uma conversa. As poucas linhas de cabeçalho técnico no topo do arquivo (entre `---`) não atrapalham a leitura; é só metadado que ferramentas com suporte a Skill sabem aproveitar e o resto ignora.

## Princípios

Três regras que não devem ser flexibilizadas em atualizações futuras:

1. **Nada de nome real.** Personas são fictícias; nenhuma sessão é atribuída a um membro específico do time.
2. **Nada de dado inventado.** Se a pesquisa não cobre, o arquivo diz que não cobre. Lacuna declarada vale mais que preenchimento plausível.
3. **Confiança é explícita.** Cada persona e cada problema carrega quantas fontes o sustentam. Quem lê precisa saber o peso do que está lendo.

Esta documentação também **não cobre como o produto funciona** — nome de feature, regra de negócio, comportamento de tela. Isso é conhecimento que muda com deploy; documentar aqui a partir de memória de reunião já causou pelo menos um erro factual, corrigido e removido. Para isso, use a fonte de verdade do produto.

## Manutenção

O Notion do time ("Mapeamento de Personas") é a fonte de verdade. Ao processar novas reuniões ou relatórios de suporte, atualize `personas.md` e `usabilidade.md` diretamente — o procedimento está descrito na última seção do `SKILL.md`.
