# Tp 1 Admin systémea

## Exercice 2. Prise en main de l’interpréteur de commandes

### Manuel

1. A l’aide du manuel, identifiez le rôle de la commande which

    ```bash
    man which
    ```

    ```txt
    DESCRIPTION
        which  renvoie le chemin des fichiers (ou liens) qui seraient exécutés  
        dans l'environnement courant si ses arguments avaient été donnés comme  
        commandes dans un interpréteur de commandes  strictement  conforme  à  
        POSIX. Pour  ce  faire, which cherche dans la variable PATH les fichiers  
        exécutables correspondant aux noms des arguments. which ne normalise pas  
        les chemins.
    ```

2. Quand on consulte une page du manuel, comment peut-on rechercher un terme (par exemple, chercher le terme option dans la page de manuel de which ?

    ```txt
    Dans le manuel, /pattern où pattern = valeur recherché
    ```

3. Comment quitte-t-on le manuel ?

    ```txt
    On appuye sur 'q' dans le manuel
    ```

4. Chaque section du manuel a une première page, qui présente le contenu de la section. Afficher la première page de la section 6 ; de quoi parle cette section ?

### Navigation dans l’arborescence des fichiers

1. Allez dans le dossier ```/var/log```

    ```bash
    cd /var/log
    ```

2. Remontez dans le dossier parent ```/var``` en utilisant un chemin relatif

    ```bash
    cd ..
    ```

3. Retournez dans le dossier personnel

    ```bash
    cd ~
    ```

4. Revenez au dossier précédent ```/var``` sans utiliser de chemin

    ```bash
    cd -
    ```

5. Essayez d’accéder au dossier ```/root```, que se passe-t-il ?

    ```bash
    -bash: cd: /root: Permission denied
    ```

6. Essayez la commande ```sudo cd /root```, que se passe-t-il ? Expliquez

    ```txt
    [sudo] password for *******:
    sudo: cd: command not found  

    cd attend un executable. cd n'est pas un executable
    ```

7. A partir de votre dossier personnel, créez l’arborescence suivante :

    ```bash
    mkdir ~/Dossier1
    touch ~/Dossier1/Fichier1
    mkdir ~/Dossier2
    mkdir ~/Dossier2/Dossier2.1
    mkdir ~/Dossier2/Dossier2.2
    touche ~/Dossier2/Dossier2.2/Fichier2
    touche ~/Dossier2/Dossier2.2/Fichier3
    ```

8. Revenez dans votre dossier personnel ; à l’aide de la commande ```rm```, essayez de supprimer Fichier1, puis Dossier1 ; que se passe-t-il ?

    ```bash
    rm ~/Dossier1/Fichier1
    rm ~/Dossier1

    rm: cannot remove 'Dossier1': Is a directory
    ```

9. Quelle commande permet de supprimer un dossier ?

    ```bash
    rmdir ~/Dossier1
    ```

10. Que se passe-t-il quand on applique cette commande à Dossier2 ?

    ```bash
    rmdir ~/Dossier2
    rmdir: failed to remove 'Dossier2': Directory not empty
    ```

11. Comment supprimer en une seule commande Dossier2 et son contenu ?

    ```bash
    rm -R ~/Dossier2
    ```

### Commandes importantes

1. Quelle commande permet d’afficher l’heure ? A quoi sert la commande time ?

    ```bash
    date
    jeudi 13 février 2020, 15:46:17 (UTC+0000)
    ```

    ```txt
    DESCRIPTION
       time run the program COMMAND with any given arguments ARG....  When COMMAND finishes,
       time displays information about resources used by COMMAND
    ```

2. Dans votre dossier personnel, tapez successivement les commandes ```ls``` puis ```la```,
que peut-on en déduire sur les fichiers commençant par un point ?

    ```txt
    ls affiche les dossiers/fichiers du repertoire courant.
    la affiche les dossiers/fichiers du repertoire courant ainsi que les dossiers/fichiers cachés.
    ```

3. Où se situe le programme ls?

    ```bash
    which ls : /usr/bin/ls
    ```

4. Essayez la commande ll. Existe-t-il une entrée de manuel pour cette commande? Utilisez les commandes alias ou aliaspour en savoir plus sur la nature de cette commande.

5. Quelle commande permet d’aﬀicher les fichiers contenus dans le dossier/bin?

6. Que fait la commandels ..?

7. Quelle commande donne le chemin complet du dossier courant?

8. Que fait la commandeecho 'yo' > plopexécutée 2 fois?

9. Que fait la commandeecho 'yo' >> plopexécutée 2 fois?

10. A quoi sert la commandefile? Essayez la sur des fichiers de types différents.

11. Créez un fichiertotoqui contient la chaîneHello Toto !; créer ensuite un lientitivers ce fichieravec la commandeln toto titi. Modifiez à présent le contenu detotoet aﬀichez le contenu detiti:qu’observe-t-on? Supprimez le fichiertoto; quelle conséquence cela a-t-il surtiti?

12. Créez à présent un lien symbolique tutu sur titi avec la commande ln -s titi tutu. Modifiez lecontenu detiti; quelle conséquence pour tutu? Et inversement? Supprimez le fichier titi; quelle conséquence cela a-t-il surtutu?

13. Aﬀichez à l’écran le fichier/var/log/syslog. Quels raccourcis clavier permettent d’interrompre etreprendre le défilement à l’écran?

14. Aﬀichez les 5 premières lignes du fichier/var/log/syslog, puis les 15 dernières, puis seulement les lignes 10 à 20.

15. Que fait la commande dmesg | less? 

16. Aﬀichez à l’écran le fichier/etc/passwd; que contient-il? Quelle commande permet d’aﬀicher la pagede manuel de ce fichier?

17. Aﬀichez seulement la première colonne triée par ordre alphabétique inverse

18. Quelle commande nous donne le nombre d’utilisateurs ayant un compte sur cette machine (pas seule-ment les utilisateurs connectés)?

19. Combien de pages de manuel comportent le mot-cléconversiondans leur description?

20. A l’aide de la commandefind, recherchez tous les fichiers se nommantpasswdprésents sur la machine

21. Modifiez la commande précédente pour que la liste des fichiers trouvés soit enregistrée dans le fichier~/list_passwd_files.txtet que les erreurs soient redirigées vers le fichier spécial/dev/null

22. Dans votre dossier personnel, utilisez la commandegreppour chercher où est défini l’aliasllvuprécédemment

23. Utilisez la commandelocatepour trouver le fichierhistory.log.

24. Créer un fichier dans votre dossier personnel puis utilisez locate pour le trouver. Apparaît-il? Pourquoi ?

## Exercice 3. Découverte de l’éditeur de texte nano

1. Copiez le fichier /var/log/syslog dans votre dossier personnel sous le nom log.txt, puis ouvrez-le avecnano

2. Remplacez toutes les occurrences du mot kernel par le mot noyau

3. Déplacer les 10 premières lignes à la fin du fichier

4. Annulez cette action

5. Enregistrez le fichier avant de quitter nano

## Exercice 4. Personnalisation du shell

1. Commencez par créer une copie de ce fichier, que vous appellerez.bashrc_bak

2. Editez le fichier.bashrcavecnanoet décommentez la ligneforce_color_prompt=yes pour activer la couleur. Enregistrez le fichier et quittez nano.

3. Le fichier.bashrc est lu au démarragedu shell; pour le recharger, il faudrait donc se déconnecter puis se reconnecter; mais il existe un autre moyen : la commandesource .bashrc. Testez-la, l’invitede commande devrait immédiatement passer en couleurs.

4. Les couleurs par défauts (surtout celle du dossier courant) ne sont pas très visibles. Dans.bashrc, cherchez les lignes commençant par PS1=; elles indiquent la mise en forme de l’invite de commande (selon que l’on est en couleurs ou non)

5. Modifiez l’invite de commande pour qu’elle s’aﬀiche sous la forme suivante: où l’heure est aﬀichée en violet et entre crochets, et le chemin du dossier courant en cyan
