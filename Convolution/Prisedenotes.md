lancement fichier

    ./convol nomImage.ras numero_filtre(de 0à4) nb-itération

Tests:

Changement filtre

    ./convol Sukhothai_4080x6132.ras 3 100
    Temps total de calcul : 67.4775 seconde(s)
    ./convol Sukhothai_4080x6132.ras 0 100
    Temps total de calcul : 80.9126 seconde(s)
    ./convol Sukhothai_4080x6132.ras 1 100
    Temps total de calcul : 83.9659 seconde(s)
    ./convol Sukhothai_4080x6132.ras 2 100
    Temps total de calcul : 70.8985 seconde(s)
    ./convol Sukhothai_4080x6132.ras 4 100
    => problème(trop long)

avec femme10.ras

    ./convol femme10.ras 3 100
    Temps total de calcul : 0.17826 seconde(s)
    ./convol femme10.ras 0 100
    Temps total de calcul : 0.208437 seconde(s)
    ./convol femme10.ras 1 100
    Temps total de calcul : 0.211496 seconde(s)
    ./convol femme10.ras 2 100
    Temps total de calcul : 0.184132 seconde(s)
    ./convol femme10.ras 4 100
    Temps total de calcul : 2.36901 seconde(s)

Changement itérations
filtre 4 image femme

    ./convol femme10.ras 4 10
    Temps total de calcul : 0.253994 seconde(s)
    ./convol femme10.ras 4 50
    Temps total de calcul : 1.19634 seconde(s)
    ./convol femme10.ras 4 500
    Temps total de calcul : 11.7843 seconde(s)
    ./convol femme10.ras 4 1000
    Temps total de calcul : 24.7374 seconde(s)

MPI

local
effets de bord

    Temps processus : 1.64228 seconde(s)
    Temps processus : 1.95911 seconde(s)
    Temps processus : 1.95842 seconde(s)
    Temps processus : 1.95813 seconde(s)
    Temps total : 1.9593 seconde(s)

sans effets

    Temps processus : 1.98481 seconde(s)
    Temps processus : 1.98598 seconde(s)
    Temps processus : 1.98177 seconde(s)
    Temps processus : 1.98241 seconde(s)
    Temps total : 1.98617 seconde(s)

Raspberry
femme 4 100

    Temps processus : 3.16515 seconde(s)
    Temps processus : 3.17685 seconde(s)
    Temps processus : 3.17784 seconde(s)
    Temps processus : 3.17607 seconde(s)
    Temps total : 3.17898 seconde(s)

Sukhotai 4080
4 0 100

    Temps processus : 105.403 seconde(s)
    Temps processus : 105.407 seconde(s)
    Temps processus : 105.439 seconde(s)
    Temps processus : 105.443 seconde(s)
    Temps total : 105.612 seconde(s)

4 1 100

    Temps processus : 105.429 seconde(s)
    Temps processus : 105.444 seconde(s)
    Temps processus : 105.47 seconde(s)
    Temps processus : 105.471 seconde(s)
    Temps total : 105.645 seconde(s)

4 2 100

    Temps processus : 53.0624 seconde(s)
    Temps processus : 53.0801 seconde(s)
    Temps processus : 53.1048 seconde(s)
    Temps processus : 53.1083 seconde(s)
    Temps total : 53.2798 seconde(s)

4 3 100

    Temps processus : 53.8166 seconde(s)
    Temps processus : 53.8304 seconde(s)
    Temps processus : 53.8778 seconde(s)
    Temps processus : 53.8869 seconde(s)
    Temps total : 54.0516 seconde(s)

4 4 100

    Temps processus : 1632.46 seconde(s)
    Temps processus : 1634.35 seconde(s)
    Temps processus : 1634.45 seconde(s)
    Temps processus : 1634.44 seconde(s)
    Temps total : 1634.85 seconde(s)

8 4 100

    Temps processus : 1460.07 seconde(s)
    Temps processus : 1482.47 seconde(s)
    Temps processus : 1483.92 seconde(s)
    Temps processus : 1484.42 seconde(s)
    Temps processus : 1487.1 seconde(s)
    Temps processus : 1488.05 seconde(s)
    Temps processus : 1488.97 seconde(s)
    Temps processus : 1489.01 seconde(s)
    Temps total : 1490.22 seconde(s)

2 2 100

    Temps processus : 101.362 seconde(s)
    Temps processus : 101.363 seconde(s)
    Temps total : 101.591 seconde(s)

8 2 100

    Temps processus : 54.1018 seconde(s)
    Temps processus : 54.1581 seconde(s)
    Temps processus : 54.1407 seconde(s)
    Temps processus : 54.1365 seconde(s)
    Temps processus : 54.2727 seconde(s)
    Temps processus : 54.3394 seconde(s)
    Temps processus : 55.2528 seconde(s)
    Temps processus : 55.3068 seconde(s)
    Temps total : 55.7453 seconde(s)

16 2 100

    Temps processus : 57.5557 seconde(s)
    Temps processus : 57.5852 seconde(s)
    Temps processus : 57.5867 seconde(s)
    Temps processus : 57.6352 seconde(s)
    Temps processus : 57.6677 seconde(s)
    Temps processus : 57.676 seconde(s)
    Temps processus : 57.7494 seconde(s)
    Temps processus : 57.7177 seconde(s)
    Temps processus : 57.7526 seconde(s)
    Temps processus : 57.8081 seconde(s)
    Temps processus : 57.8349 seconde(s)
    Temps processus : 58.0872 seconde(s)
    Temps processus : 58.2199 seconde(s)
    Temps processus : 58.1289 seconde(s)
    Temps processus : 60.4168 seconde(s)
    Temps processus : 60.4849 seconde(s)
    Temps total : 61.3817 seconde(s)

32 2 100

    erreur : la hauteur = 4080 n'est pas un multiple de p = 32 !

8 2 10

    Temps processus : 5.96698 seconde(s)
    Temps processus : 6.02241 seconde(s)
    Temps processus : 6.03391 seconde(s)
    Temps processus : 6.03811 seconde(s)
    Temps processus : 6.20698 seconde(s)
    Temps processus : 6.32791 seconde(s)
    Temps processus : 6.39997 seconde(s)
    Temps processus : 6.4195 seconde(s)
    Temps total : 6.74346 seconde(s)

8 2 1000

    Temps processus : 529.783 seconde(s)
    Temps processus : 529.773 seconde(s)
    Temps processus : 529.779 seconde(s)
    Temps processus : 529.834 seconde(s)
    Temps processus : 529.863 seconde(s)
    Temps processus : 529.879 seconde(s)
    Temps processus : 530.284 seconde(s)
    Temps processus : 530.165 seconde(s)
    Temps total : 530.638 seconde(s)

8 2 10000

    Temps processus : 7632.56 seconde(s)
    Temps processus : 7633.07 seconde(s)
    Temps processus : 7633.06 seconde(s)
    Temps processus : 7633.19 seconde(s)
    Temps processus : 7633.23 seconde(s)
    Temps processus : 7633.21 seconde(s)
    Temps processus : 7633.56 seconde(s)
    Temps processus : 7633.44 seconde(s)
    Temps total : 7634 seconde(s)
