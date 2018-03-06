# kubernetes-playaround

## Gcloud Commands

`gcloud auth login` To login using your google account

`gcloud container clusters get-credentials -z asia-east1-b project-name` if you have already signed in using your gcloud CLI then this project will get the credentials from gcloud to that cluster and connect to itk

`gcloud config set container/use_client_certificate False`

## Kubectl Commands

`kubectl proxy` opens a gateway to the kubernetes cluster you have configured on your localhost

`kubectl config get-contexts` that will show you which clusters you *can* connect to, as well as which one is the current context

`kubectl get pods -n namespace` get the pods you have access to

`kubectl get services`

`kubectl describe svc mongo`

`kubectl describe po mongo-deployment-<guid>-<guid>`

`kubectl exec -it pod-name bash --namespace=namespace` use the terminal in a particular pod

`kubectl port-forward pod-name 27000:27017` forward port for pod

`kubectl get ing` get ingress services