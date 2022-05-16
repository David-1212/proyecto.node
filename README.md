Alumno: Vargas López David Guadalupe.
 GitHub:
1.-Clonar el repositorio (con el comando “git clone https://github.com/David-1212/proyect”) Docker (Tomando 	en cuenta que se clono el repositorio de github con todos los archivos de este.)
2.-Subir el api a DockerHub
3.-Se utiliza el comando “docker-compose up” para verificar que esté funcionando correctamente. 
Kubernetes:
4.-minikube start
5.-kompose convert (solo en caso de no tener los archivos. yaml del repositorio de GitHub
6.-kubectl apply -f • api-deployment.yaml • api-service.yaml • webmvc-deployment.yaml • webmvc-	service.yaml
7.-kubectl get pods
8.-kubectl get services
9.-kubectl port-forward api 3000:3000
10.-kubectl port-forward webmvc-api 4001:4001
11.-minikube dashboard
12.-minikube dashboard --url 
Istio
13.-Si no se tiene istio, instalar istioctl.
14.-Comprobar la instalación con el comando “istioctl”
15.-Comando injected: kubectl label namespace default istio-injection=enabled
16.-Aplicar los servicios tal como se hizo anteriormente en el paso 3 de Kubernetes.
17.-Con el commando “kubectl port-forward kiali -n istio-system 20001” se hace llamada a kiali dentro del puerto 20001
18.-Acceder en el navegador a localhost:20001
