# Install Nginx Ingress Controller on AWS

## Step 1: Deploy the below manifest

```bash
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.11.1/deploy/static/provider/aws/deploy.yaml
```

---

# prerequisites

kubectl – A command line tool for working with Kubernetes clusters. For more information, see [Installing or updating kubectl]("https://docs.aws.amazon.com/eks/latest/userguide/install-kubectl.html").

eksctl – A command line tool for working with EKS clusters that automates many individual tasks. For more information, see [Installing or updating]("https://docs.aws.amazon.com/eks/latest/userguide/eksctl.html").

AWS CLI – A command line tool for working with AWS services, including Amazon EKS. For more information, see [Installing, updating, and uninstalling the AWS CLI]("https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-install.html") in the AWS Command Line Interface User Guide. After installing the AWS CLI, we recommend that you also configure it. For more information, see [Quick configuration]("https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html#cli-configure-quickstart-config") with aws configure in the AWS Command Line Interface User Guide.

---

# Install EKS

Please follow the prerequisites doc before this.

## Install a EKS cluster with EKSCTL

```
eksctl create cluster --name demo-cluster --region us-east-1 
```

## Delete the cluster

```
eksctl delete cluster --name demo-cluster --region us-east-1
```

---