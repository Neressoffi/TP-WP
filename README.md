/*Ce projet a eter lancer sans le Docker vu mon pb de machine */
  1- Premiere étape:

     -creation et configuration du fichier : .env 
          (a l'interieur renseigner ces differents elements:
                 IP=127.0.0.1
                 DB_ROOT_PASSWORD=root
                 DB_NAME=wp)
   2-Deuxieme étape Creation de la base de donner wp avec phpmyadmin:
      -importation des données du fichier data.sql
      
   3-configuration du du fichier wp-config.php :  
        /** le nom de ma dataBase et les acces  */
        define( 'DB_NAME', 'wp');

        /** Database username */
        define( 'DB_USER', 'root');

        /** Database password */
        define( 'DB_PASSWORD', null);
   4-Lancer le serveur php en executant la commande :
    
    -php -S localhost:80 -t ./wp-app  (lancement sur le port 80 vu que j'ai mis le     lancement d'APAH en pause)
    -php -S localhost:8000 -t ./wp-app

    5-Augmentation de la vitesse d'exection de la serveur(configuration dans mon PhpMyadmin)
