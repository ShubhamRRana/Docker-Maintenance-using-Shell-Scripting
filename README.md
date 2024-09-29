Hi all,

In this repository we have learned how we can automate the process of cleaning the docker of unused images, containers and volumes.
This method of cleaning is used becuase it saves us the hassle of manually finding which images, containers and volumes are not in use and can be removed just by runnig a single shell script file, removing all the images, containers and volumes. 

Step - 1 :
Before executing the file make sure the script has executable permissions.

![image](https://github.com/user-attachments/assets/1ce7c7fb-cbaa-419c-89ae-fb3b22118d9c)

Step - 2 :
Use command "./docker_clean.sh -h", this shows what commands can be used with the ./docker_clean.sh command

![image](https://github.com/user-attachments/assets/f69e235d-2a00-488c-baee-aeb63b16f0a2)

In the above image you can see two commands,
i) ./docker_clean.sh --dry-run => This command shows what are the changes it's going to make to the docker images, containers and volumes. 
ii) ./docker_clean.sh => This command makes all the changes displayed in the above command.

Step - 3 : 
Here we can see what are the changes we are going to perform.

![image](https://github.com/user-attachments/assets/fcdec7d0-c15b-4692-baf7-ed30db01e3e2)

For reference check the image id and container id we are deleting.

![image](https://github.com/user-attachments/assets/18acf4ac-199f-4f4b-888d-0dd44277b2a6)

![image](https://github.com/user-attachments/assets/a9183004-56a5-4e46-8594-bb2a58fc7ca9)

Step - 4 :

Here we can see changes being made in action.

![image](https://github.com/user-attachments/assets/003f86c1-aa46-4e20-9228-a197635adc3e)

Checking if the changes made are reflected back in the docker.

![image](https://github.com/user-attachments/assets/8a761ade-1727-437a-b082-201cd76f714e)

![image](https://github.com/user-attachments/assets/58e621e1-8a29-45ff-9471-8ee6e91a77fd)

As we can see the script has been successfully executed removing all the unused images, containers and volumes.
