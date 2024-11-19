---
title: Nintendo
sidebar_position: 2
---

Les consoles de jeux ne prennent pas en charge le DNS crypté, mais elles sont bien adaptées à la configuration de l'AdGuard DNS public ou de l'AdGuard DNS privé via une adresse IP liée.

Il est probable que votre routeur prenne en charge l'utilisation de serveurs DNS cryptés, vous pouvez donc toujours configurer l'AdGuard DNS privé dessus et connecter votre console de jeux à celui-ci.

[Comment configurer votre routeur](/private-dns/connect-devices/routers/routers.md)

:::note Compatibilité

S'applique à : New Nintendo 3DS, New Nintendo 3DS XL, New Nintendo 2DS XL, Nintendo 3DS, Nintendo 3DS XL et Nintendo 2DS.

:::

## Connectez AdGuard DNS

Configurez votre console de jeux pour utiliser un serveur DNS AdGuard public ou configurez-la via IP liée :

1. Dans le menu d'accueil, sélectionnez _Paramètres système_.
2. Accédez aux _Paramètres Internet_ → _Paramètres de connexion_.
3. Sélectionnez le fichier de connexion, puis sélectionnez _Modifier les paramètres_.
4. Sélectionnez _DNS_ → _Configuration_.
5. Réglez _Auto-Obtention du DNS_ sur _Non_.
6. Sélectionnez _Configuration détaillée_ → _DNS principal_. Maintenez la flèche gauche enfoncée pour supprimer le DNS existant.
7. Dans le champ _Serveur DNS_, saisissez l'une des adresses de serveur DNS suivantes :
   - `94.140.14.49`
   - `94.140.14.59`
8. Enregistrez les paramètres.

Il serait préférable d'utiliser une IP liée (ou une IP dédiée si vous avez un abonnement Équipe) :

- [IP dédiées](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [IP liées](/private-dns/connect-devices/other-options/linked-ip.md)