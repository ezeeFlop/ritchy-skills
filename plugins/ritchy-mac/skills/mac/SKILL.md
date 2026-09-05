---
name: mac
description: Agir sur l'ordinateur de Christophe — afficher une image ou une page, lire ses mails, décrire son écran, lancer un raccourci, mener une tâche web. À activer dès que la demande concerne « mon ordi », « mon écran », « mes mails », « affiche », « ouvre », « va sur », « remplis ».
tools: mcp.mac.mac_show mcp.mac.mac_open_url mcp.mac.mac_screenshot mcp.mac.mac_mail_recent mcp.mac.mac_mail_read mcp.mac.mac_notify mcp.mac.mac_run_shortcut mcp.mac.mac_clipboard_get mcp.mac.mac_clipboard_set mcp.mac.mac_browse
---

# Le Mac de Christophe

- Afficher / ouvrir : `mac_show` (fichier ou URL) ou `mac_open_url`. Réponds « c'est affiché » en une phrase.
- Mails : `mac_mail_recent` (5) puis, si demandé, `mac_mail_read` N. Résume chaque mail en une phrase parlée, jamais de lecture intégrale sauf demande explicite.
- « Qu'est-ce qu'il y a sur mon écran ? » : `mac_screenshot` et redis la description.
- Une image que tu viens de générer : passe son chemin ou son URL à `mac_show`.
- ACTIONS (raccourci, presse-papiers, tâche web `mac_browse`) : demande d'abord « je le fais ? » et n'agis qu'après un oui. `mac_browse` peut durer une minute : dis « je m'en occupe » et laisse le résultat revenir au tour suivant. Un objectif web = une phrase précise avec le site.
