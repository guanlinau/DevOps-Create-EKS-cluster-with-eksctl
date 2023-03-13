### Create EKS cluster with eksctl

### Technologies Used:

Kubernetes, AWS EKS, Eksctl, Linux

### Project Description:

1- Create EKS cluster using eksctl tool that reduces the manual effort of creating an EKS cluster

### Instructions:

###### Step 1: Install eksctl

```
brew tap weaveworks/tap
```

```
brew install weaveworks/tap/eksctl
```

### Step 2: Configure eksctl login credentials

```
aws configure
```

### Step 3: Create eks cluster by eksctl

```
❯ eksctl create cluster \
> --name aws-cluster \
> --version 1.17 \
> --region au-southeast-2 \
> --nodegroup-name aws-cluster-nodes \
> --node-type t2.micro \
> --nodes 2 \
> --nodes-min 1 \
> --nodes-max 3
```
