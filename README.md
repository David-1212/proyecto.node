# Proyecto v1

Es un proyecto realizado en node.js con el fin de ejemplificar el uso de docker, kubernetes(minikube), ademas de istio y cheekymonkey.

## GitHub 🚀
```
1.-Clonar el repositorio (con el comando “git clone https://github.com/David-1212/proyect”) Docker (Tomando 	en cuenta que se clono el repositorio de github con todos los archivos de este.)
```

### Kubernetes: 📋


```
2.-minikube start
3.-kompose convert (solo en caso de no tener los archivos. yaml del repositorio de GitHub)
4.-kubectl apply -f 
	• api-deployment.yaml 
	• api-service.yaml 
	• webmvc-deployment.yaml 
	• webmvc-service.yaml
5.-kubectl get pods
6.-kubectl get services
7.-kubectl port-forward api 3000:3000
8.-kubectl port-forward webmvc-api 4001:4001
9.-minikube dashboard
10.-minikube dashboard --url 
```

### Istio 🔧

```
11.-Si no se tiene istio, instalar istioctl.
12.-Comprobar la instalación con el comando “istioctl”
13.-Comando injected: kubectl label namespace default istio-injection=enabled
14.-Aplicar los servicios tal como se hizo anteriormente en el paso 3 de Kubernetes.
15.-Con el commando “kubectl port-forward kiali -n istio-system 20001” se hace llamada a kiali dentro del 	puerto 20001
16.-Acceder en el navegador a localhost:20001
```

## cheekymonkey ⚙️

```
17.- Instalar los requerimentos con el comando "pip install -r requirements.txt"
18.- utilizar el comando "python cheekymonkey.py --exclude kube-system cert-manager istio-system" para correr el programa
```

###Elaborado por: ⌨️



```
Vargas López David Guadalupe
```
