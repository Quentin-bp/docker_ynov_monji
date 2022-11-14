BARBOSA Thomas

YEYE Axel

BOMPARD Quentin

VIANA Enzo

Importation de l'image python :


On créé le Dockerfile : 


![image](https://user-images.githubusercontent.com/73823634/201684831-c36e0ae9-ae7e-44d0-a2b6-1c7a144ef846.png)


On utilise l'image de départ python:3.6-alpine que notre image héritera avec la commande FROM, puis l'on installe flask (version 1.1.2) avec RUN. On instancie ensuite les deux variables d'environnement avec la commande ENV.
Pour terminer, on expose le port 8080 avec la commande EXPOSE qui sera le port utilisé par défault, et on lance la commande python app.py lors de la construction de l'image.


![image](https://user-images.githubusercontent.com/73823634/201686551-582de7b6-379f-4a53-8db8-bd9281102bdb.png)


![image](https://user-images.githubusercontent.com/73823634/201686584-af2b81ed-f058-47b4-b76e-884a280416bc.png)
