# GKE create - Tech With Nishant

### List all Projects
```
gcloud projects list
```
### Set Project
```
gcloud config set project <project-id>
```
### Set the default region so you dont need to pass to every command
```
gcloud confing set compute/zone us-east1-d
```
### Create a Cluster: (You can even pass the compute size but we are going with default
```
gcloud container cluster create <cluster-name> \
	 --node-pool=default-pool \
	 --region=us-east1
```
