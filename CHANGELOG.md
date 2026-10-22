# Nouveautés de Zaphir (anciennement Dat00u)

## 0.19.0 — le guide des programmes pour toutes les sources

- **Listes M3U :** une liste qui indique son guide des programmes (fichier XMLTV, `url-tvg` ou `x-tvg-url`) l'affiche maintenant, sans rien régler : le programme en cours sous chaque chaîne, avec sa progression, dans la mosaïque, la liste sur l'image et le menu de la chaîne (en cours, à suivre, « Programmes »).
- **Démo :** le guide aussi. Parmi la centaine de fichiers que la liste Free-TV indique, seuls ceux des pays de ses chaînes sont lus (six au plus).
- **Réglages › Chaînes TV › Guide des programmes :**
  - l'état du guide : nombre de chaînes trouvées, heure de mise à jour, fichiers qui n'ont pas pu être lus ; OK le télécharge de nouveau ;
  - deux guides publics de [XMLTV Fr](https://xmltvfr.fr), désactivés tant que vous ne les choisissez pas : « TNT » (0,7 Mo par jour) et « France » (environ 400 chaînes, 9 Mo par jour) ;
  - « Ajouter l'adresse d'un guide » : celui de votre fournisseur ou un autre guide public (.xml ou .xml.gz).
- **Abonnements Xtream :** les programmes viennent toujours du serveur ; un guide ajouté complète les chaînes qui n'en ont pas.
- **Les chaînes sont retrouvées** par leur identifiant de guide, sinon par leur nom, comme pour les logos ; un nom trop courant (« Sport 1 ») ne suffit pas, et le pays écrit avec le nom doit être le bon.
- **Léger :** le guide est téléchargé au plus une fois par jour, en arrière-plan, et gardé sur l'appareil ; si le site est en panne, celui de la veille reste. La journée à venir de chaque chaîne est gardée, avec une limite de taille et de mémoire pour les petites box.
- **Site et présentation :** la liste de ce que l'application contacte est complétée (annuaire de logos, guides, démo).

**English — 0.19.0:** the TV guide for every source. An M3U list that names its XMLTV guide now shows what's on (and next) everywhere, the demo too. Settings › TV channels › TV guide shows its state and offers two public XMLTV Fr guides (off until chosen) and an "Add a guide address" option; on Xtream, an added guide fills the channels the server leaves empty. Downloaded at most once a day in the background, kept on the device.

## 0.18.0 — plus rapide, réglages et recherche refaits

- **Grosses listes plus rapides.** Mesuré sur une liste de 75 000 contenus : réouverture en 8 à 15 s au lieu de 27 s, premier chargement en 22 s au lieu de 32 s, et l'écran ne se fige plus pendant la préparation.
  - La liste enregistrée sert une semaine (au lieu de 12 heures) et se met à jour en arrière-plan.
  - Pendant l'attente, l'écran dit où en est le chargement : « Téléchargement… 4,2 Mo », « Lecture… 37 888 contenus », « Préparation de la liste… ».
  - Un téléchargement coupé est relancé une fois automatiquement.
  - 19 Mo de mémoire en moins : les textes répétés d'un contenu à l'autre ne sont plus gardés en double.
- **Réglages (TV) :**
  - ← → parcourent les choix et **OK** choisit : une flèche ne change plus un réglage toute seule. ← avant le premier choix revient au menu, sur la catégorie affichée.
  - Plus de grand titre : un fil « Réglages › Lecture ». L'aide s'affiche sur la ligne sélectionnée, et « D'autres réglages plus bas » quand la page continue.
  - La reconnexion et la mémoire tampon rejoignent « Lecture », à côté du profil de lecture ; « Direct et guide » devient « Chaînes TV ».
  - Sources : la source utilisée en tête, avec son nombre de chaînes, de films et de séries ; « Retirer » devient une petite icône, qui demande toujours confirmation.
- **Recherche :**
  - Les meilleurs résultats d'abord : le nom de la chaîne ou du film, puis le dossier, le genre, les acteurs et le résumé.
  - Une rangée par type (chaînes, films, séries), avec « Tout voir » ; sous un résultat trouvé autrement que par son nom, la raison (« Dossier FR | Sport », « Genre : Sport »…).
  - Les filtres n'apparaissent qu'avec des résultats ; pendant la recherche, « Recherche dans … contenus » (le nombre de votre liste) remplace « 0 résultat ».
- **Plus clair :**
  - Les onglets Films et Séries disparaissent quand la source n'en a pas ; l'accueil n'affiche plus de bannière vide et rappelle la source et son nombre de chaînes.
  - Le direct est un point rouge dans le coin : l'étiquette cachait le nom des chaînes sans logo.
  - Le bouton d'une série lance l'épisode suivant non vu et le nomme (« Reprendre · S1 · E3 »).
  - Sur TV, à la première chaîne regardée, un rappel des touches (OK, Retour, ↑ ↓) s'affiche une seule fois.
  - Ajout de source : le nom du serveur est proposé quand « Mon abonnement » est déjà pris ; un bouton inactif est gris.
- **Grandes listes de dossiers (TV) :** quand la plupart des dossiers commencent par un pays (« FR | Sport »), une rangée « Tous · FR · BE · CH… » les filtre.
- **Téléphone :** les onglets passent en bas de l'écran, avec icônes ; dans le lecteur de films et d'épisodes, glisser à gauche règle la luminosité, à droite le volume.
- **Corrections :** le message d'une chaîne en panne ne passe plus devant la liste des chaînes ; « Vérifié il y a 2 minutes » sans majuscule au milieu de la phrase ; une liste de plus de 48 Mo explique quoi demander au fournisseur.

**English — 0.18.0:** much faster with large lists (reopening in 8–15 s instead of 27 s on a 75,000-item list), loading steps shown. TV settings: arrows move over the choices and OK picks, so an arrow never changes a setting by itself; a lighter page with help on the selected row. Search ranks name matches first, shows one row per type with "See all" and says why a result matched. Country filters on long folder lists, bottom tabs and brightness/volume swipes on phones, and several fixes.

## 0.17.0 — essayer sans abonnement

- **Essayer sans abonnement :** sur l'écran de connexion, sous Xtream, Lien M3U et Fichier, le bouton « Essayer sans abonnement » ouvre une démo de chaînes gratuites.
  - Les chaînes viennent de la liste publique [Free-TV/IPTV](https://github.com/Free-TV/IPTV), qui ne recense que des chaînes gratuites et légales ; Zaphir n'en héberge aucune et la lit à son adresse, donc ses corrections arrivent sans nouvelle version.
  - Huit dossiers : France, Infos, Infos (arabe), Liban, Émirats, Égypte, Qatar, Arabie saoudite. Les liens YouTube, que le lecteur ne peut pas lire, sont retirés.
  - Une capsule « Démo » rappelle d'où viennent les chaînes et où ajouter les vôtres (Réglages › Sources). La démo se retire comme une autre source, et le bouton disparaît une fois qu'elle est ajoutée.
  - Comme toute liste publique, certaines chaînes peuvent être en panne ou bloquées selon le pays : le message habituel s'affiche alors.

**English — 0.17.0:** "Try without a subscription" on the connection screen opens a demo of free channels from the public Free-TV/IPTV list (France, news, Arab world), read at its address; YouTube links are left out and a "Demo" capsule says where to add your own source.

## 0.16.0 — une liste des chaînes plus simple

- **Retour remonte d'un étage (TV) :** on ne se perd plus dans la liste des chaînes.
  - Une chaîne s'ouvre avec son bandeau (nom, qualité, programme) ; **OK** ouvre le menu de la chaîne (pause, programmes, favori, qualité, audio, sous-titres, réglages).
  - **Retour** ferme le menu, puis ouvre la liste des chaînes sur la chaîne regardée, puis la liste des dossiers ; un dernier **Retour** ramène à la mosaïque.
  - Dans les dossiers, ↑ ↓ montrent tout de suite les chaînes de chaque dossier ; **OK** ou → y entre. En haut de la liste, « ‹ Dossiers · Sport · 2/11 » dit où l'on est.
  - ← ouvre toujours la liste en plein écran, et les dossiers depuis la liste. ← → ne font plus défiler les dossiers un par un.
  - Fermer la liste sans choisir de chaîne ne change pas de dossier : elle se rouvre toujours sur la chaîne regardée.
- **Bandeau :** après la liste, le bandeau de la nouvelle chaîne s'affiche seul, sans rouvrir les boutons.
- **Site :** la page de téléchargement reprend le logo, le slogan et les couleurs de l'appli.

**English — 0.16.0:** on TV, Back now climbs one level at a time: channel menu, picture, channel list, folders, then the mosaic. Folders are listed beside the channels and previewed as you move; ← → no longer cycle through folders one by one. The download page now uses the app's logo and colours.

## 0.15.0 — la liste des chaînes sur l'image

- **Liste des chaînes sur l'image (TV) :** une chaîne s'ouvre directement en plein écran, avec la liste de son dossier par-dessus l'image, sur un quart de l'écran. Elle remplace la vue réduite (vidéo en petit à côté de la liste).
  - ↑ ↓ choisissent une chaîne, ← → changent de dossier, OK lance la chaîne et ferme la liste.
  - En plein écran, ← rouvre la liste sur la chaîne regardée ; Retour la ferme, puis ramène à la mosaïque sur la chaîne regardée.
  - Chaque ligne montre le numéro, le logo, le nom et le programme en cours (ou le nombre de qualités) ; la chaîne qui joue a un point rouge.
  - Sur une tablette, un bouton « Chaînes » dans les commandes ouvre la liste.
- **Favoris :** « Zapper seulement dans les favoris » est désormais activé par défaut, sur tous les appareils ; il reste désactivable dans les réglages.
- **Ouverture :** l'écran du logo reste deux secondes et ne laisse plus apparaître un instant l'écran de connexion avant l'accueil.

**English — 0.15.0:** on TV, channels open full screen with the channel list over the picture (replacing the reduced view); zapping through favourites is on by default; the logo screen stays two seconds and no longer flashes the connection screen.

## 0.14.0 — nouveau logo, image figée

- **Nouveau logo :** un Z à facettes, menthe et bleu saphir, autour d'un triangle de lecture, et le slogan **« Zappez, trouvez votre saphir. »**. Il apparaît sur l'icône de l'appli, la bannière Android TV, l'écran d'ouverture et le menu. L'écran d'ouverture reste au moins une seconde et demie pour qu'on le voie.
- **Image figée :** quand une chaîne charge sans fin, s'arrête ou garde la même image alors que le son continue, la qualité suivante prend le relais toute seule (« Image figée : passage en HD ») ; une chaîne en une seule qualité est relancée au direct. Au plus trois fois par minute, puis le message d'erreur habituel. Réglages › Direct et guide › « Changer de qualité si l'image se fige ».
- **Fenêtres :** plus fines, en verre, avec des boutons arrondis ; seul le bouton sélectionné est coloré, on ne peut plus confondre « Rester » et « Quitter ». Une action risquée (retirer une source…) ne devient rouge qu'au moment où on la sélectionne.
- **Messages :** une fine capsule centrée avec un point de couleur (vert, ambre, rouge, bleu) ; pendant une vidéo, elle s'affiche en haut pour ne pas cacher le lecteur.
- **Petit lecteur :** « Reconnexion » s'affiche dans une capsule sur l'image ; quand une chaîne ne répond plus, l'image s'assombrit avec un message court.

**English — 0.14.0:** new faceted Z logo and slogan, automatic quality switch when the picture freezes (or a restart), finer dialogs where only the focused button is filled, thin message capsules, cleaner messages in the small player.

## 0.13.0 — un lecteur modernisé

- **Barre en verre :** à chaque changement de chaîne, une barre discrète en bas de l'image montre le logo, le numéro, la qualité (FHD, HD…) et l'heure.
  - Avec le guide des programmes : le programme en cours, jusqu'à quelle heure, et la suite.
  - Sans guide, le cas le plus courant : le dossier et la position (« 2/7 »), l'image et le son du flux (« 1080p · Stéréo »), et les chaînes vers lesquelles mènent ↑ et ↓.
- **Commandes :** OK agrandit la même barre avec Pause, Favori et, si la chaîne en a un, le Guide ; à droite, des boutons ronds pour l'audio, les sous-titres, la qualité et les réglages.
- **Panneau de réglages :** audio, sous-titres, qualité, format d'image (et vitesse pour les films) dans un seul panneau à droite ; ← / → changent d'onglet, l'image reste visible.
- **Films et séries :** la même barre, des boutons −10 s / +10 s, et l'heure visée s'affiche au-dessus du curseur pendant le déplacement.
- **Chargement :** le logo de la chaîne et la qualité essayée s'affichent pendant la connexion, au lieu d'un écran noir.
- **Erreurs :** une carte claire dit quelles qualités ont été essayées, avec « Réessayer » et « Chaîne suivante ».
- **Repères :** Pause / Lecture et ±10 s s'affichent un instant au milieu de l'image, y compris avec la touche ▶❚❚ de la télécommande.
- **Correction :** l'indicateur de chargement s'affiche de nouveau après un changement de chaîne.

**English — 0.13.0:** a modernised player: a slim glass bar with logo, quality and clock (programme with a TV guide, folder, stream details and neighbouring channels without one), a side panel for audio, subtitles, quality and picture format, a loading screen with the channel's logo, clear error cards with "Retry" and "Next channel", and on-screen play/pause and ±10 s signs.

## 0.12.0 — une tuile par chaîne

- **Qualités regroupées :** une chaîne proposée en LOW, SD, HD, FHD ou 4K n'a plus qu'une tuile, avec le nombre de qualités sous son nom. Les dossiers beIN passent par exemple de 65 à 26 tuiles.
  - La meilleure qualité est lancée (FHD, puis HD, 4K, SD, LOW) ; si elle ne passe pas, la suivante prend le relais toute seule (« Passage en HD »).
  - Le bouton de qualité du lecteur liste les qualités de la chaîne ; le choix est retenu.
  - Le zapping passe d'une chaîne à l'autre, plus d'une qualité à l'autre.
  - Ne sont jamais regroupées : une autre langue (« beIN SPORT 1 FR »), un décalage (« TF1+1 ») ou un autre numéro.
- **Dossiers de qualité :** les dossiers « … HD / FHD / 4K » que l'appli remplissait elle-même ne sont plus remplis : ils répétaient le dossier complet.
- **Favoris et récents :** une chaîne mise en favori dans une qualité s'affiche sur la tuile regroupée.
- **Réglage :** Réglages › Direct et guide › « Regrouper les qualités » (activé par défaut) pour revenir à l'ancien affichage.
- **Tuiles sans logo :** initiales plus lisibles sur les petites tuiles.

**English — 0.12.0:** one tile per channel: LOW/SD/HD/FHD/4K qualities are grouped, the best one plays and the next takes over if it fails, quality menu in the player, quality folders no longer duplicated, favourites follow the grouped tile.

## 0.11.2 — logos, réglés sur un vrai abonnement

- **Beaucoup plus de logos reconnus**, avec des règles mises au point sur un abonnement réel de 1 500 chaînes :
  - le chiffre collé à la qualité (« Arryadia 1HD ») et « Sport » ou « Sports » ;
  - la plateforme devant le nom (« OSN ART AFLAM 1 »), les noms plus longs dans l'annuaire (« beIN MOVIES 2 » est « beIN Movies 2 Action ») ;
  - les noms arabes écrits autrement (« Kuwait TV 1 » est KTV 1, « janoubia », « Zaytoona », « Al Hiwar Al Tunisi ») ;
  - la version d'un pays (« Rotana Cinema » prend Rotana Cinema KSA ou Egypt).
- **Moins d'erreurs :** le pays du dossier ou du nom doit correspondre (une chaîne syrienne ne prend plus le logo d'une chaîne saoudienne), et une faute n'est tolérée qu'après le début du nom (« MBC » n'est jamais « MNC »).
- **Logo de la marque en dernier recours :** « Roya Sport » prend le logo de Roya TV, « TF1+1 » celui de TF1, « CANAL+ LIVE 9 » celui de Canal+.
- **Sans aucun logo :** une tuile neutre avec le nom de la chaîne écrit en entier et un liseré menthe remplace les initiales sur fond de couleur.

**English — 0.11.2:** many more channel logos recognised (tuned on a real 1,500-channel subscription), fewer wrong logos, the brand's logo as a last resort, and a neat name tile when there is no logo.

## 0.11.1 — plus de logos reconnus

- **Logos :** l'annuaire public passe désormais en premier ; le logo de votre abonnement ne sert que si l'annuaire ne connaît pas la chaîne. Réglages › Apparence › « Logos depuis internet ».
- **Plus de chaînes reconnues :**
  - un mot courant en moins : « beIN News » trouve « beIN Sports News » ;
  - un numéro que l'annuaire ne connaît pas prend le logo de sa famille : « beIN SPORT 9 » prend celui de beIN Sports ;
  - la langue ou le pays autour du nom : « beIN SPORTS 1 Arabic », « FR TF1 », « TF1 FR » ;
  - les noms écrits dans une autre langue : « Tunisia nat 1 » trouve El Watania 1.

**English — 0.11.1:** the public logo directory now comes first and recognises more channels (beIN, Arabic and Maghreb channels, names written differently).

## 0.11.0 — logos des chaînes

- **Logos des chaînes :** quand votre abonnement ne donne pas le logo d'une chaîne, ou qu'il ne s'affiche pas, Zaphir le cherche dans un annuaire public de chaînes (iptv-org). Les petites fautes dans les noms sont tolérées (« Canal+ Sprot », « Eurosprot 2 ») ; le pays écrit dans le nom ou le dossier (« FR: », « |AR| ») aide à choisir. Sans correspondance sûre, la chaîne garde ses initiales. Réglages › Apparence › « Logos manquants depuis internet » permet de le couper.
- **Logos :** ils sont posés sur un fond neutre, la couleur est réservée aux initiales.
- **Thème Ardoise :** plus profond, toujours aussi lisible.
- **Dossiers :** en sélection multiple, les dossiers déplacés restent visibles sous la barre d'actions et la sélection n'est plus perdue. Au téléphone, le dossier en déplacement a ses boutons ▲ ▼ ✓.
- **TV :** dans la vue réduite, Retour remonte d'abord au choix du dossier, puis à la mosaïque.

**English — 0.11.0:** channel logos found automatically when your subscription has none (spelling mistakes tolerated), deeper Slate theme, easier folder moving (touch buttons on phones), Back in reduced live TV goes to the folder choice first.

## 0.10.0 — Dat00u devient Zaphir

- **Nouvelle identité :** l'application s'appelle **Zaphir**, signée *by dat00u*, avec un nouveau logo Z. C'est la même application : la mise à jour s'installe par-dessus, vos sources, favoris et réglages sont conservés.
- **Thèmes :** deux thèmes soignés, **Ardoise** (par défaut, gris-bleu lumineux) et **Clair**. Si vous utilisiez un ancien thème, l'application choisit automatiquement le plus proche.
- **Accueil :** une grande image avec « Regarder » et « Détails », la rangée « Reprendre » avec le temps restant, puis vos favoris.
- **Navigation :** menu en haut (Accueil, TV, Films, Séries, Favoris), sélection entourée de menthe, bien visible à la télécommande.
- **TV :** chaînes sur 3 colonnes, repère « EN DIRECT » rouge ; dans la vue réduite, un seul Retour ramène à la mosaïque sur la chaîne regardée.
- **Sécurité :** les mises à jour sont vérifiées par leur empreinte avant installation ; les erreurs de code PIN sont comptées même après la fermeture de l'application ; l'ajout d'une source depuis le téléphone est mieux protégé.
- **Textes :** « 1 chaîne / 15 chaînes » et les formes arabes correctes.

**English — 0.10.0:** Dat00u becomes Zaphir (by dat00u): new logo, Slate and Light themes, new home screen, clearer remote navigation, red LIVE marker, fingerprint-checked updates, stronger PIN and phone-link protection.

## 0.9.2 — thèmes et fluidité

- **Thèmes :** cinq thèmes dans Réglages › Apparence.
  - **Dat00u sombre :** celui d'avant.
  - **Aurore :** fond sombre avec halos de couleur, boutons arrondis.
  - **Cinéma :** l'affiche du film ou de la série sélectionnée remplit le fond.
  - **Studio clair :** thème clair, sélection entourée de noir.
  - **Néon OLED :** noir pur, halo de couleur autour de la sélection.
  - Le lecteur reste sombre dans tous les thèmes. Si vous aviez Noir OLED, Graphite ou Bleu nuit, l'application choisit le thème le plus proche.
- **Télécommande :** le focus arrive toujours au bon endroit (menu, dossiers, grilles) et ne se perd plus après une action ; le lecteur réduit du direct est atteignable, OK le passe en plein écran.
- **Dossiers :** chaque dossier a son menu (déplacer, épingler, masquer) et la sélection multiple permet d'agir sur plusieurs à la fois.
- **Mises à jour :** une fenêtre au milieu de l'écran annonce la nouvelle version au démarrage ; la vérification manuelle garde le focus et affiche le résultat sur place.
- **Fluidité :** moins de calculs à chaque déplacement dans les grilles.

**English — 0.9.2:** five themes (Dat00u dark, Aurora, Cinema, Light studio, Neon OLED), better remote focus, folder menus with multiple selection, centered update window, smoother grids.

## 0.9.1 — contrôle des mises à jour

- **Mises à jour :** cette version sert à vérifier que la mise à jour automatique fonctionne depuis la 0.9.0. Aucun changement visible ; vos sources, favoris et réglages sont conservés.

**English — 0.9.1:** update check release, no visible change.

## 0.9.0 — première version distribuée

- **Mises à jour :** l'application vous prévient quand une nouvelle version est disponible. Sur TV, elle la télécharge et l'installe elle-même. Une section « Mises à jour » est ajoutée dans Réglages › À propos.
- **Appareils :** une seule application pour Android TV, Google TV, Fire TV, les box, les téléphones, les tablettes, les pliables et les Chromebook. L'interface s'adapte à l'écran.
- **Téléphone :**
  - les dossiers d'abord, en liste ou en mosaïque ;
  - le contenu en liste ou en mosaïque ;
  - le mini-lecteur du direct, avec changement de dossier sans couper l'image ;
  - le balayage vers le haut ou le bas pour changer de chaîne en plein écran ;
  - l'image dans l'image.
- **Direct :**
  - un dossier « Favoris » ;
  - les programmes du jour dans le menu de la chaîne, avec le replay quand la chaîne le permet ;
  - les noms de dossiers lisibles sur deux lignes.
- **Dossiers :** ordre personnalisable, déplacement d'un dossier ou d'un groupe, épingler, masquer, rechercher.
- **Démarrage rapide :** la liste enregistrée s'affiche tout de suite, l'abonnement est vérifié en arrière-plan, et les films et séries se chargent discrètement.
- **Navigation :**
  - Retour mène à la fiche après un film ou un épisode, puis au menu avant de proposer de quitter ;
  - la télécommande est plus fluide ;
  - le nouveau logo est en place.
- **Corrections :** saisons et épisodes, cartes coupées par le zoom, réglages allégés, et nombreux détails d'affichage.

**English — 0.9.0:** update checks with in-app install on TV, one app for every Android device, phone layout with list or mosaic views, favourites folder and programme list in the live channel menu, folder ordering, faster start, smoother navigation and many fixes.
