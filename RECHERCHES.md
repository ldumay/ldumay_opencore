[Retour](../../)

# Recherches supplémentaires

## OpenCore

### Recherche 1 - vérifier la version de opencore

- [google - vérifier la version de opencore](https://www.google.com/search?rlz=1C1CHBF_frFR912FR912&sxsrf=AJOqlzUKSaMgm1RPEB_xC4-Q_NLokIMr4A:1678188394624&q=v%C3%A9rifier+la+version+de+opencore&spell=1&sa=X&ved=2ahUKEwj9v4L52sn9AhXSVKQEHao5ChsQBSgAegQIOxAB&biw=3072&bih=1586&dpr=1.25)
  - [Connaitre sa version OpenCore](https://www.hackintosh-montreal.com/t11338-connaitre-sa-version-opencore)
  - [How to check current OpenCore version?](https://www.reddit.com/r/hackintosh/comments/guqvft/how_to_check_current_opencore_version/)
  - [Unable to verify my version of Open Core](https://www.tonymacx86.com/threads/unable-to-verify-my-version-of-open-core.310371/)

Solution 1

```
nvram 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102:opencore-version
```

Solution 2

```
nvram 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102:opencore-version -p > ~/Desktop/opencore-version.txt
```

Solution 3

```
Dans votre config.plist, définissez ExposeSensitiveData sur 15.
```

Solution 4

```
Ouvrez votre dossier OC, accédez à votre OpenCore.efi et faites un clic droit dessus. Sélectionnez Obtenir des informations dans la liste déroulante, vérifiez et notez la date de création et non de modification.

OpenCore est publié sur une base mensuelle.

Par exemple, la version 0.6.3 est sortie début novembre, chaque version suivante est sortie un mois plus tard. Alors...

0.6.0 - Août 2020
0.6.1 - Septembre 2020
0.6.2 - Octobre 2020
0.6.3 - Novembre 2020
0.6.4 - Décembre 2020
0.6.5 - Janvier 2021
0.6.6 - Février 2021

Si le Get info date de création tombe dans un mois particulier, le numéro de version doit être issu de la liste ci-dessus.
```