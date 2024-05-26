Instalación local Kubernetes con MicroK8s
    • sudo snap install microk8s --classic
    • microk8s enable dns
    • microk8s enable dashboard
    • microk8s enable storage
Se debe instalar de kubctl para la administración del cluster
Se crea un namespace llamado dev 
Se crean dos archivos manifiestos en yaml
deployment.yaml
my-app-config.yaml
En el archivo deployment.yaml construirá y levantará los pods, servicios y volumes; mientras que el archivo my-app-config.yaml será el configmaps.
Primero se corre el deployment del my-app-config.yaml y luego se podrá comprobar que hay en el sistema antes de aplicar el deployment
Después de la aplicación de deployment se podrá realizar un test: Eliminación de pod y creación automática del mismo.
Exposición de la aplicación y acceso mediante un navegador: http://localhost:8083/
