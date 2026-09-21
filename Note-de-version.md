# 7.0.0 (2026-09-18) préversion

## AZERTY DCS

L’AZERTY zéro prise de tête est maintenant disponible en préversion, car au niveau logiciel tout est pleinement fonctionnel, mais tout n’est pas complet depuis la sortie d’Unicode 18.0 l’avant-veille, avec 160 nouvelles lettres latines (et 19 autres caractères) à prendre en charge. Manque aussi une documentation à jour et complète.

DCS, c’est "débogué, complété, semi-automatique". Ce qui est débogué, c’est le verrouillage Majuscule, qui ne met plus en accès direct ni le point d’interrogation, ni le symbole livre, ni le symbole micro, ni la touche morte tréma, mais qui met en Majuscule les capitales des minuscules accentuées de notre clavier, et l’espace fine insécable qui sert de séparateur des milliers. « Complété » par la prise en charge de l’écriture latine au niveau d’Unicode 17.0, de 1 125 symboles mathématiques et de quelques autres dont 155 émojis (codés sur moins de 4 octets). Les 26 lettres émojis (pour les sites et navigateurs qui affichent les drapeaux) sont en AltEm, la touche modificatrice ajoutée sur la touche de verrouillage Majuscule. « Semi‑automatique » au sens où les grandes ponctuations "?;:!" sont déjà espacées (par la fine insécable) en AltGr sur leurs touches, les guillemets "«»‹›" aussi (ou pas) en AltGr ou Maj + AltGr sur les six touches qui restent à droite. 

Zéro prise de tête parce que tout d’abord, ce qui est marqué sur les touches reste là où c’est marqué. Ensuite, sur 30 des 31 touches mortes, on peut appuyer 2, 3 ou 4 fois pour voir s’afficher le caractère mort. Pas sur la touche morte groupe, en AltGr sur accent circonflexe/tréma et sur Maj + AltGr + Q (pour la synergie avec les touches mortes en Maj + AltGr), parce que sous Windows, elle parcourt les 12 groupes indéfiniment (mais faire suivre le chiffre permet d’abréger, avec 0 à 2 pour 10 à 12). Et si une position de touche n’insère pas de caractère visible, on peut faire afficher quelque chose en la faisant précéder de la touche morte accent circonflexe ; sauf pour l’espace nulle sur Maj + AltGr + T, utilisée pour insérer les demi-codets hauts : "𐞥" ⇐ AltGr + A (touche morte exposant), Maj + AltGr + T (espace nulle), AltGr + A (touche morte exposant), q). Cela fonctionne aussi pour les trois points à mi-hauteur : le point médian sur AltGr + R, le point d’hyphénation sur AltGr + Z, et l’opérateur point sur AltGr + C.

Une fois que la documentation est mise à jour et complétée, il y aura des vues de disposition. De toute manière, le marquage des touches est 100 % respecté.

L’AZERTY DCS est la variante rétrocompatible de l’AZERTY complet qui, lui, est encore plus logique et plus facile à utiliser. Certes au prix de quelques disruptions, mais la virgule et toutes les lettres du français sont inchangées, et les grandes ponctuations restent sur leurs touches (?;:!) ou sont ajoutées à la place de "%", "µ", "£" et tréma qui prend la place de "(", qui va sur AltGr + D.


