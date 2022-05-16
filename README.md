Alumno: Vargas López David Guadalupe.
 GitHub
	Clonar el repositorio (con el comando “git clone https://github.com/David-1212/proyect”) Docker (Tomando 	en cuenta que se clono el repositorio de github con todos los archivos de este.)
	Subir el api a DockerHub
	Se utiliza el comando “docker-compose up” para verificar que esté funcionando correctamente. 
Kubernetes:
	minikube start
	kompose convert (solo en caso de no tener los archivos. yaml del repositorio de GitHub)
	kubectl apply -f • api-deployment.yaml • api-service.yaml • webmvc-deployment.yaml • webmvc-	service.yaml
	kubectl get pods
	kubectl get services
	kubectl port-forward api 3000:3000
	kubectl port-forward webmvc-api 4001:4001
	minikube dashboard
	minikube dashboard --url 
Istio
	Si no se tiene istio, instalar istioctl.
	Comprobar la instalación con el comando “istioctl”
	Comando injected: kubectl label namespace default istio-injection=enabled
	Aplicar los servicios tal como se hizo anteriormente en el paso 3 de Kubernetes.
	Con el commando “kubectl port-forward kiali -n istio-system 20001” se hace llamada a kiali dentro del 	puerto 20001
	Acceder en el navegador a localhost:20001
