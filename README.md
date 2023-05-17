# K8s-on-EKS

Just a simple project for setting up Kubernetes on Amazon Elastic Kubernetes Service (EKS)


# 1. Set up an AWS account and create an IAM user with the necessary permissions to create an EKS cluster. 
## You will need the AmazonEKSClusterPolicy and AmazonEKSServicePolicy IAM policies attached to the user.

# 2. Install and configure the AWS CLI (Command Line Interface) on your local machine. You can find the installation instructions for the AWS CLI [here](https://aws.amazon.com/pt/cli/)

# 3. Create an Amazon EKS cluster by using the AWS CLI or the AWS Management Console.

To create a cluster using the AWS CLI, use the eksctl create cluster command. For example:

- `eksctl create cluster --name my-eks-cluster --region us-west-2 --nodegroup-name my-node-group --node-type t2.micro --nodes 3`

This command creates an EKS cluster named my-eks-cluster in the us-west-2 region with a node group named my-node-group. 
The node group consists of three EC2 instances of type t2.micro.

To create a cluster using the AWS Management Console, follow the instructions in the Amazon EKS Getting Started guide [here](https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html)

# 4. Install and configure kubectl, the Kubernetes command-line tool, on your local machine. You can find the installation instructions for kubectl [here](https://kubernetes.io/docs/tasks/tools/)

$ 5. Verify that kubectl can connect to your EKS cluster by running the following command:

- `kubectl get nodes`

This command lists the nodes in your EKS cluster.

Once you have installed Kubernetes on EKS, you can start deploying and managing containerized applications on the cluster. You can use kubectl to create and manage Kubernetes resources, such as deployments, services, and pods. You can also use tools like Helm and Kubernetes Operators to manage more complex applications on your EKS cluster.

For more information, see the [Amazon EKS documentation](https://aws.amazon.com/pt/eks/)
