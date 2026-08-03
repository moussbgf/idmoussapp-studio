# idmoussapp-studio

Site public d'**Idmoussapp Studio**, servi par GitHub Pages :
<https://moussbgf.github.io/idmoussapp-studio/>

Il n'existe que pour une raison : la Play Console et AdMob exigent que la politique de
confidentialité soit accessible à une **URL publique**. Les dépôts de code des applications sont
**privés**, et GitHub Pages ne publie pas depuis un dépôt privé sur l'offre GitHub Free — d'où ce
dépôt public séparé, qui ne contient aucun code.

## Contenu

| Chemin | URL publique | Source de vérité |
|---|---|---|
| `dirham-rial/index.html` | <https://moussbgf.github.io/idmoussapp-studio/dirham-rial/> | `docs/privacy/index.html` du dépôt privé `dirhamrialmarocaineuro` |

## ⚠️ Ce dépôt est une COPIE, pas la source

La politique de confidentialité doit décrire ce que l'application fait **réellement**. Elle est donc
écrite et versionnée **avec le code**, dans le dépôt privé de l'application, où une modification
touchant aux données (nouveau SDK, nouvelle requête réseau, nouveau stockage) se voit dans le même
commit.

Ici, ce n'est qu'un miroir. **Les fichiers doivent rester rigoureusement identiques** — ne jamais
éditer la copie directement, sinon l'URL publique se met à décrire une application qui n'existe pas.

Republier après toute modification de la source :

```bash
cp /c/projets/app/dirhamrialmarocaineuro/docs/privacy/index.html /c/projets/idmoussapp-studio/dirham-rial/index.html
```

Vérifier que les deux sont en phase — aucune sortie signifie qu'ils sont identiques :

```bash
diff /c/projets/app/dirhamrialmarocaineuro/docs/privacy/index.html /c/projets/idmoussapp-studio/dirham-rial/index.html
```

C'est aussi la raison pour laquelle la copie ne porte **aucune mention** signalant qu'elle est une
copie : le moindre écart volontaire rendrait ce `diff` inutilisable.

## Ajouter une application

Un sous-dossier par application, nommé d'après elle, contenant un `index.html`. Ajouter la ligne
correspondante au tableau ci-dessus et à la liste de la page d'accueil.

## Notes

- `.nojekyll` désactive le traitement Jekyll : ces pages sont du HTML statique autonome, sans
  dépendance externe (ni police, ni feuille de style, ni script).
- Aucun contenu de ce dépôt n'est confidentiel. Ne rien y déposer qui ne soit destiné à être public.
