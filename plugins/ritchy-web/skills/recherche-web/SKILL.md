---
name: recherche-web
description: Chercher une information récente sur le web et répondre en deux phrases avec la source. À activer dès que la question porte sur l'actualité, un produit, une version, un prix, une définition que la mémoire ne connaît pas.
tools: mcp.web.searxng_web_search mcp.web.web_url_read
---

# Recherche web (voix)

1. Reformule la question en 3 à 6 mots-clés (langue de la source probable : anglais pour la tech).
2. Appelle `mcp.web.searxng_web_search` avec ces mots-clés, `count` 5.
3. Choisis au plus DEUX résultats crédibles (site officiel, dépôt GitHub, documentation, presse reconnue). Ignore les forums de spam.
4. Lis-en un avec `mcp.web.web_url_read` seulement si le résumé du résultat ne suffit pas.
5. Réponds en DEUX phrases parlées maximum, puis nomme la source en un mot (« d'après GitHub », « selon la doc Pollen »). Pas de liste, pas d'URL prononcée.
6. Si rien de fiable : dis-le en une phrase et propose de chercher autrement.
