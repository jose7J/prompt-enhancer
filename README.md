# prompt-enhancer

> **Transforme qualquer prompt em um prompt de elite — em segundos.**

Uma Claude Skill que pega qualquer instrução — por mais vaga, curta ou confusa
que seja — e a reescreve como um prompt profissional e de alto desempenho,
aplicando as melhores técnicas de engenharia de prompt.

---

## Por que isso importa

A qualidade da sua resposta depende 90% da qualidade do seu prompt.
Um prompt vago gera resposta genérica. Um prompt de elite gera resultado de elite.

Esta skill faz a engenharia de prompt por você:

- Detecta o domínio (criativo, técnico, analítico, operacional...)
- Aplica os **8 pilares** de um prompt de alto desempenho
- Usa técnicas avançadas como **Chain of Thought**, **few-shot** e **structured output**
- Marca suposições explicitamente para você corrigir se necessário
- Entrega diagnóstico com pontuação do prompt original e melhorado

---

## O que faz

| Etapa | O que acontece |
|-------|----------------|
| 1. Classifica o domínio | Criativo / Técnico / Analítico / Operacional / Acadêmico / Conversacional |
| 2. Avalia o prompt (1–10) | Clareza, Contexto, Formato, Objetivo, Acionabilidade |
| 3. Aplica 8 pilares | Persona, Missão, Contexto, Passos, Formato, Exemplos, Restrições, Critérios |
| 4. Aplica técnicas avançadas | CoT, Few-shot, Structured output, Negative prompting, Metacognição |
| 5. Preenche lacunas | Suposições razoáveis marcadas como `[SUPOSIÇÃO: ...]` |
| 6. Entrega com diagnóstico | Prompt melhorado + pontuação + o que mudou + refinamentos |

---

## Antes e depois

**Antes:**
> "faz um texto pra vender ingles"

**Depois:**
> *Você é um copywriter de resposta direta com especialização em edtech e growth
> marketing. Escreva 3 variações de copy para WhatsApp (máximo 6 linhas cada)
> promovendo um curso de inglês online para adultos profissionais [SUPOSIÇÃO:
> faixa 25–45 anos, B2C, ticket médio R$ 200/mês]. Estrutura obrigatória: (1)
> gancho com dor emocional, (2) benefício transformacional, (3) CTA com urgência.
> Tom: consultivo, sem agressividade...*

---

## Instalação

### macOS / Linux

```bash
git clone https://github.com/<seu-usuario>/prompt-enhancer.git
cp -r prompt-enhancer ~/.claude/skills/prompt-enhancer
```

### Windows (PowerShell)

```powershell
git clone https://github.com/<seu-usuario>/prompt-enhancer.git
Copy-Item -Recurse prompt-enhancer "$env:USERPROFILE\.claude\skills\prompt-enhancer"
```

Reinicie o Claude Code — a skill é carregada automaticamente.

---

## Como usar

Basta pedir em linguagem natural. Exemplos que ativam a skill:

| O que você diz | O que acontece |
|----------------|----------------|
| `"melhora esse prompt: [seu prompt]"` | Reescreve com os 8 pilares |
| `"deixa esse prompt perfeito"` | Aplica todas as técnicas relevantes |
| `"otimiza pra eu ter a melhor resposta"` | Adiciona CoT, formato, critérios |
| `"como eu deveria perguntar sobre X?"` | Constrói o prompt do zero |
| `"prompt engineering para Y"` | Cria prompt especializado para o domínio |
| `"turbina esse pedido"` | Versão turbo com técnicas avançadas |

---

## Técnicas aplicadas

| Técnica | Quando é usada | Benefício |
|---------|----------------|-----------|
| **Chain of Thought** | Tarefas analíticas/técnicas complexas | Reduz erros de raciocínio |
| **Few-shot examples** | Padrão de saída não é óbvio | Alinha o formato esperado |
| **Structured output** | Dados, tabelas, JSONs | Resultado reutilizável |
| **Negative prompting** | Evitar desvios comuns | Reduz saídas fora do escopo |
| **Metacognição** | Incertezas e ambiguidades | Modelo sinaliza quando não sabe |
| **Self-consistency** | Múltiplas abordagens válidas | Comparação de alternativas |
| **Verificação interna** | Requisitos complexos | Reduz omissões e alucinações |

---

## Dicas para melhores resultados

- **Mais contexto = mais precisão.** Mesmo um prompt ruim melhora muito com
  qualquer informação adicional que você fornecer.
- **Corrija as `[SUPOSIÇÕES]`.** A skill sinaliza o que assumiu — substitua
  pelo que é real no seu caso.
- **Use o diagnóstico.** A pontuação original vs. melhorada mostra exatamente
  onde o prompt original tinha pontos cegos.
- **Refine iterativamente.** Responda às perguntas de refinamento para ir de
  "ótimo" para "perfeito".

---

## Estrutura

```
prompt-enhancer/
├── SKILL.md      # Lógica da skill, processo e exemplos
└── README.md     # Este arquivo
```

---

## Licença

MIT — use, modifique e distribua livremente.
