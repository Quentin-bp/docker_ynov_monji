BARBOSA Thomas

YEYE Axel

BOMPARD Quentin

VIANA Enzo

PROUCHANDY Thomas


1/

Importation de l'image python :


On créé le Dockerfile : 

![image](https://user-images.githubusercontent.com/73823634/201700930-e4394fb7-f2fa-4a12-94d4-93a805aaf008.png)


On utilise l'image de départ python:3.6-alpine que notre image héritera avec la commande FROM, puis l'on installe flask (version 1.1.2) avec RUN. On instancie ensuite les deux variables d'environnement avec la commande ENV.
Pour terminer, on expose le port 8080 avec la commande EXPOSE qui sera le port utilisé par défault, et on lance la commande python app.py lors de la construction de l'image.


![image](https://user-images.githubusercontent.com/73823634/201686551-582de7b6-379f-4a53-8db8-bd9281102bdb.png)


![image](https://user-images.githubusercontent.com/73823634/201686584-af2b81ed-f058-47b4-b76e-884a280416bc.png)


2/

On importe la dernière version de docker registry
![image](https://user-images.githubusercontent.com/73823634/201696690-5212ccac-4b4f-4bd4-a304-171fa44fa95b.png)


![image](https://user-images.githubusercontent.com/73823634/201697103-d862cf20-3696-4e85-93ad-b8164c9a45d1.png)


![image](https://user-images.githubusercontent.com/73823634/201697164-3189db39-2151-46ea-950b-f095d13f6340.png)

![image](https://user-images.githubusercontent.com/73823634/201697415-f968ce15-dec6-4670-a4c5-aeee59d70ce2.png)


On vérifie que le container 
![image](https://user-images.githubusercontent.com/73823634/201697570-78d448e0-f881-4544-a20a-5258f5780e7f.png)

Enfin, on le met dans docker hub :

![image](https://user-images.githubusercontent.com/111991074/201730073-227e5696-a0bf-4238-a498-7871ccb75b1a.png)


3/

On créé le fichier docker-compose.yaml avec le contenu suivant : 

![image](https://user-images.githubusercontent.com/111991074/201728354-ad966492-470c-4636-8d85-5c6bd041ad1e.png)

On lance le script avec les 4 images en cours de création :
![image](https://user-images.githubusercontent.com/111991074/201728432-b81d52a5-43af-4c33-a1a1-bd1f5af3b00c.png)

Voici le résultat :

![image](https://user-images.githubusercontent.com/111991074/201728670-83dccbce-7749-4ca7-a833-2629072ca380.png)

![image](https://user-images.githubusercontent.com/111991074/201728717-79046e04-2263-4221-8b0d-c381bbf6f45f.png)

![image](https://user-images.githubusercontent.com/111991074/201728760-93d337d4-8b3a-45f9-b29f-c9747f621ddc.png)






