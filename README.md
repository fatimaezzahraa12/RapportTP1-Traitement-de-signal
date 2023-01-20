# RapportTP1-Traitement-de-signal

Réalisé par :Fatima Ezzahraa Chadni

# Thème :Analyse Spectrale d'un signal et étude de la Transformée de Fourrier Discrète.

Objectifs:
- Représentation de signaux et applications de la transformée de Fourier discrète
(TFD) sous Matlab. 
-Evaluation de l’intérêt du passage du domaine temporel au domaine fréquentiel 
dans l’analyse et l’interprétation des signaux physiques réels.

-Travail Demandé:
Réaliser un script Matlab commenté qui contient le travail réalisé avec les représentations graphique expliquées sur le travail Effectué.

# Manipulation 1:Représentation temporelle et fréquentielle .

-On considère un signal sinusouidal composé de trois fréquences dont les valeurs sont respectivement 440 Hz,550Hz et 2500Hz.
La première opération à faire est effectuer un échantillonnage du signal avec une fréquence d'échantillonage de 10000Hz.Pour ceci ,on prend 5000 valeurs qui représentent le nombre d'échantillons souhaités.

  ![image](https://user-images.githubusercontent.com/120644217/213785578-e12e3f78-3d32-4683-9a80-a00ee00ac640.png)
  
  Après cette étape,on génère le bruit Gaussien suivant une loi Normale Centrée Réduite à l'aide de la commande randn().
  On ajoute le bruit à notre signal d'origine puis on applique la transformée de Fourrier à notre signal en utilisant la commande fft().
  On utilise une fréquence fshift dont la valeur est représentée dans le script.On utilise aussi la commande fftshift() pour centre notre spectre fréquentiel et         normaliser les valeurs obtenues.
  
  ![image](https://user-images.githubusercontent.com/120644217/213805097-f012e996-5150-4d7d-a4c8-2bd5e0b0708f.png)

  Comme on peut observer clairement  sur le graphe 3 pics.Ces pics représentent exactement les fréquenes contenues dans notre signal.On augmente ensuite l'intensité     du bruit pour visualiser son effet sur   le signal en représentation fréquentielle.
  ![image](https://user-images.githubusercontent.com/120644217/213787187-09fde1a6-c971-4515-8d30-2a766ca79e7b.png)
  
  # Manipulation 2:Analyse fréquentielle du chant du rorqual bleu
  À travers cette manipulaion,notre objectif est de détecter à travers une analyse de Fourier le contenu fréquentiel d’une onde sonore émise pas un rorqual bleu.
  Premièrement,on charge le fichier qui contient le son du rorqual bleu à travers la commande audioread(),puis on récupère le son  correspondant aux indices 
  allant de 2.45e4 à 3.10e4 .Pour cela, on utilise la commande chant=signal(2.45e4,3.10e4).
  L'étape suivante consiste à définir l'intervalle de fréquence et appliquer la transformée de Fourrier au signal pour le représenter au domaine fréquentiel.
     
  ![image](https://user-images.githubusercontent.com/120644217/213807048-597128ba-6e88-41ac-8973-516b8576b8b1.png)

  # Représentation du signal du rorqual bleu dans le domaine temporel.
  ![image](https://user-images.githubusercontent.com/120644217/213807779-55bea21f-83e4-4a42-a75d-e94b84d69794.png)
   # Représentation du signal du rorqual bleu dans le domaine fréquentiel.
   Comme on peut observer dans la figure ci-dessus,le spectre du signal représentent des pics, ces Pics représentent les valeurs de fréquence que contient le chant du    rorqual bleu.
   
   ![image](https://user-images.githubusercontent.com/120644217/213808209-090a442a-8368-41cc-aa04-abacc5c61692.png)

  
