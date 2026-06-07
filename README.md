# prompt-enhancer

Uma **Claude Skill** que transforma qualquer prompt — mesmo o pior, mais vago ou mal
escrito — em um prompt **excelente, estruturado e completo**, para garantir a melhor
resposta possível do modelo.

> Pegue um prompt ruim → receba um prompt perfeito → garanta a resposta perfeita.

## O que faz

Ao ativar, a skill:

1. **Diagnostica** o que falta no prompt (objetivo, contexto, formato, tom, critérios).
2. Reescreve aplicando os **7 pilares de um prompt excelente** (papel, tarefa, contexto,
   passos, formato de saída, restrições/exemplos, critérios de qualidade).
3. Preenche lacunas com **suposições explícitas** marcadas como `[SUPOSIÇÃO: ...]`.
4. Entrega o **prompt melhorado pronto para copiar** + explicação do que mudou +
   perguntas opcionais de refinamento.

## Instalação

### Como skill pessoal (Claude Code)

Copie a pasta para o diretório de skills do Claude Code:

```bash
git clone https://github.com/<seu-usuario>/prompt-enhancer.git
cp -r prompt-enhancer ~/.claude/skills/prompt-enhancer
```

No Windows (PowerShell):

```powershell
git clone https://github.com/<seu-usuario>/prompt-enhancer.git
Copy-Item -Recurse prompt-enhancer "$env:USERPROFILE\.claude\skills\prompt-enhancer"
```

Reinicie o Claude Code e a skill será carregada automaticamente.

## Como usar

Basta mencionar ou pedir, por exemplo:

- "melhora esse prompt: faz um texto pra vender ingles"
- "deixa esse prompt perfeito"
- "otimiza esse pedido pra eu ter a melhor resposta"

## Estrutura

```
prompt-enhancer/
├── SKILL.md      # Instruções e metadados que o Claude carrega
└── README.md     # Este arquivo
```

## Licença

MIT
