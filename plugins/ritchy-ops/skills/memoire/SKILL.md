---
name: memoire
description: Protocole de recherche dans la mémoire long-terme de Christophe quand la première recherche ne suffit pas — entités d'abord, faits ensuite, dates citées, franchise si absent.
tools: memory.search mcp.spongram-spongram.search_nodes
---

# Mémoire long-terme

1. Nomme l'entité au cœur de la question (personne, société, projet, outil). Appelle `mcp.spongram-spongram.search_nodes` avec son nom seul, `scope` `{"all": true}` : la fiche porte le savoir consolidé.
2. Si la fiche ne répond pas, appelle `memory.search` avec entité + sujet (« Sponge Theory banque »), puis une reformulation si besoin. Deux essais maximum.
3. Réponds en une ou deux phrases, cite la date du fait quand elle existe (« depuis juillet »).
4. Si rien : « Je ne l'ai pas en mémoire, tu veux que je le note ? » Si Christophe donne la valeur, écris-la avec `memory.add` en une phrase autonome nommant l'entité.
