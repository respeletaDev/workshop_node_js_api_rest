# NODE JS (API Rest)
Entorno de ejecución para JavaScript construido con el motor de JavaScript V8 de Chrome.

![](https://cdn-images-1.medium.com/max/1600/1*22I1ecGbrdPjGuKYTvkdWw.png)

## Node JS

-   ¿Qué es Node.js?
    -   Node.js es un entorno JavaScript del lado del servidor, basado en eventos. 
    -   Node ejecuta JavaScript utilizando el motor V8, desarrollado por Google para uso de su navegador Chrome. 
    -   Aprovechando el motor V8 permite a Node proporciona un entorno de ejecución del lado del servidor que compila y ejecuta JavaScript a velocidades increíbles. 
El aumento de velocidad es importante debido a que V8 compila JavaScript en código de máquina nativo, en lugar de interpretarlo o ejecutarlo como bytecode. 
Node es de código abierto, y se ejecuta en Mac OS X, Windows y Linux.

-   ¿Qué podemos hacer con Node.js?
    Con Node.js tenemos la posibilidad de realizar un amplio número de aplicaciones, entre las que se destacan: 
    -   Aplicaciones Web
    -   Aplicaciones de consola
    -   Chats
    -   Proxis
    
-   Instalación
    -   Node.js cuenta con un instalador pre-compilado para las plataformas mas comunes: Windows - MacOs - Linux    
    -   [Descargar](https://nodejs.org/es/download/)
    
-   [NPM (Node Package Manager)](https://www.npmjs.com/)
    -   Es el gestor de paquetes javascript de Node.js por excelencia. Gracias a él, tenemos casi cualquier librería disponible a tan solo una linea de comando de distancia, permitiéndonos utilizarla en cuestión de segundos.
    -   NPM utiliza el archivo package.json para almacenar todos los datos relevantes a nuestra aplicación. Así que lo primero que tenemos que hacer es iniciar con el comando:

            npm init
    -   Para descargar e instalar una dependencia especificada con NPM utilizamos:

            npm install `nombreDelPaquete` 
            
        Alternativas
        

            npm install `nombreDelPaquete@version` 
            npm install `nombreDelPaquete` --save  
            npm install `nombreDelPaquete` -g
            
    -   Para ejecutar el archivo principal del proyecto:

            npm start
            
-   Hola Mundo!
-   FrameWorks
![Framework](https://raw.githubusercontent.com/Unitech/PM2/development/pres/cluster-support.png) 

## Express
-   ¿Que es Express? 
-   Nuestra primera API Rest 

## Escalabilidad
![Escalabilidad](https://blog.forocoin.net/wp-content/uploads/2018/06/Sharding-Escalabilidad.jpeg)

-   Estructuración de carpetas del proyecto
-   [PM2](https://github.com/Unitech/pm2) 

## WorksShop  


    3   Run the bootstrap script:          

        -    Login as the user `zcebjobs` and Create the file `deploy.sh` and copy the content of the file `bootstrap.sh`

        -   Give permissions to the file to run as shell

           `chmod +x deploy.sh`
        
        -   Run the script    

            `sudo sh deploy.sh`  


- Login in to the centos server 

- Go to the project directory
    
      cd /var/www/

- Pull the recent master changes from the repo `This depends on the enviroment your are deploying (dev-branch, integration or master)`

      git checkout master
      git pull

- Download the node dependecies

      cd api
      npm install
      cd ..

      cd logger
      npm install
      cd ..

