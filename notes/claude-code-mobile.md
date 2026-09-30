# Claude Code sur téléphone — journal

## Séance 1 (30/09/2026)

### Ce qu'on a compris
- **Claude Code sur téléphone** (app Claude, onglet Code, ou claude.ai/code) tourne
  dans le cloud, sur une copie d'un dépôt GitHub. D'où l'obligation de passer par GitHub.
- Dans ce mode, Claude **ne peut pas toucher au téléphone** (réglages, applis, fichiers).
  Il ne travaille que sur les fichiers du dépôt.
- **Sur PC**, Claude Code tourne sur la machine : il peut agir sur la configuration.
- Pour agir sur le téléphone : Claude Code **sur PC** + téléphone branché en USB + **ADB**.
  - Sur l'A40 : Options pour les développeurs → Débogage USB activé.
  - **scrcpy** (déjà utilisé avec succès) : affiche et pilote l'écran du téléphone sur le PC.
- Termux (terminal Linux sur Android) : possible mais limité (pas d'accès aux réglages
  système sans root). Non conseillé pour débuter.

### Garder le fil entre les séances
- Les conversations restent dans la liste des sessions (app Claude → Code, ou
  claude.ai/code) : on peut rouvrir une ancienne session et continuer à écrire dedans.
- Sur PC : `claude --continue` reprend la dernière conversation, `claude --resume`
  permet d'en choisir une.
- Ce journal + `CLAUDE.md` servent de mémoire durable, quel que soit l'appareil.

### Prochaines étapes possibles
- [ ] Fusionner cette branche dans `main` pour que `CLAUDE.md` soit lu automatiquement
      par les nouvelles sessions.
- [ ] Faire un premier petit projet depuis le téléphone pour tester le fonctionnement.
- [ ] Sur PC : refaire scrcpy + ADB avec Claude Code pour régler le téléphone.
