# Como instalar: Criar jogos com o Claude

## Jeito rápido (Claude Code)
Rode no terminal, dentro da pasta do seu jogo:

```bash
npx skills add gamedev-skills/awesome-gamedev-agent-skills
```

Isso instala as 77 skills de game dev e o router. Precisa do Node.js 22.20 ou mais novo.

Prefere como plugin do Claude?

```bash
claude plugin marketplace add gamedev-skills/awesome-gamedev-agent-skills
claude plugin install gamedev@awesome-gamedev-agent-skills
```

## Esta skill (o guia em português)
**Claude.ai ou Claude Desktop:** Configurações → Capacidades → Skills → envie `criar-jogos-com-ia.zip`, sem descompactar.
**Claude Code:** descompacte e copie a pasta `criar-jogos-com-ia` para `~/.claude/skills/` (todos os projetos) ou `.claude/skills/` (um projeto). Abra uma sessão nova.

## Conferir
Pergunte: "Você tem a skill criar-jogos-com-ia?". Depois, faça o primeiro pedido de `COMO-USAR.md`.

O repositório original é github.com/gamedev-skills/awesome-gamedev-agent-skills (Apache-2.0). Conferido em 10/11/2026.
