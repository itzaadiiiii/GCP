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
<!-- - **`gcloud container clusters create day2-ops`:** Calls the Google Cloud CLI to provision a managed Kubernetes cluster named `day2-ops`.
- **`-region=us-east1`:** Deploys the cluster as a **regional cluster** across multiple availability zones in South Carolina (`us-east1`). Regional clusters replicate the Kubernetes control plane across zones for higher availability.
- **`-num-nodes=1`:** Sets the node count to 1 **per zone**. Because `us-east1` has three availability zones (`us-east1-b`, `us-east1-c`, and `us-east1-d`), this flag creates **3 worker nodes total** (1 in each zone).

#### You can go to GKE UI and see provisioning

- By default it took **`e2 medium`** size as we not provided.
- Go to Compute Engine you can see it created 3 compute engines **`one per zone`** in region **`us-east1`** -->
