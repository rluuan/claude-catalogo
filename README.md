# claude-catalogo

Meu catálogo de plugins e skills para o Claude, em português. Alguns são meus, outros são traduções de projetos de outras pessoas, sempre com o crédito e a licença original.

## Catálogo

| Plugin | O que faz | Origem |
|---|---|---|
| [humanizer](plugins/humanizer) | Tira as marcas de escrita de IA de um texto | Tradução de [blader/humanizer](https://github.com/blader/humanizer) (MIT) |

## Instalar

No Claude Code, adicione o catálogo uma vez:

```
/plugin marketplace add rluuan/claude-catalogo
```

Depois instale o que quiser:

```
/plugin install humanizer@claude-catalogo
```

Para atualizar quando eu mexer em alguma coisa:

```
/plugin marketplace update claude-catalogo
```

## Skill, plugin e marketplace

- **Skill** é uma pasta com um arquivo `SKILL.md`: instruções que o Claude carrega quando a tarefa combina com a descrição dela. Dá para usar sozinha, copiando a pasta para `~/.claude/skills/`.
- **Plugin** é um pacote que pode ter skills, comandos, agentes, hooks e servidores MCP. Facilita instalar, atualizar e desligar tudo junto.
- **Marketplace** é um repositório que lista plugins. Este repo é um.

## Estrutura

```
.claude-plugin/marketplace.json   lista de plugins do catálogo
plugins/<nome>/
  .claude-plugin/plugin.json      dados do plugin
  skills/<nome>/SKILL.md          a skill em si
  LICENSE                         licença do autor original, quando for tradução
```

Para adicionar um item novo: criar a pasta em `plugins/`, colocar na lista do `marketplace.json` e na tabela acima.
