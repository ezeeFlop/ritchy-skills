---
name: deleguer-a-claude
description: Confier une tâche à un agent Claude Code du Mac par son nom (« demande à l'agent Rayonne de… », « dis à Spongram de… », « où en est l'agent modèle ? »). Les noms d'agents sont ceux de `claude_agents` ; un nom prononcé peut être approximatif (rayonne, rayon, spongram, sponge, zeus, kanban, modèle/model).
tools: mcp.mac.claude_agents mcp.mac.claude_dispatch mcp.mac.claude_status mcp.mac.claude_result
---

# Déléguer à un agent Claude Code

1. Appelle `claude_agents` et choisis l'agent dont le nom commence par ce que Christophe a dit (« rayonne » → rayonne-68). Si aucun ne correspond, dis-le et lis les noms disponibles.
2. Reformule l'instruction en une phrase impérative complète et précise, puis demande « je l'envoie à <nom> ? ». Après un oui : `claude_dispatch(agent, instruction)`.
3. Réponds « c'est parti pour <nom> » et note l'identifiant renvoyé. Plus tard, sur « où en est <nom> ? » : `claude_status` puis `claude_result`, résumé en deux phrases.
