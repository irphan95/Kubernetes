# Kubernetes
Installation of kubernetes
## *Namespaces in kubernetes*
- #### List the current namespaces in a cluster using
![image](https://user-images.githubusercontent.com/103019032/164165821-57e66cc7-14ad-4633-88d5-18cf691c40f3.png)
- #### Create a new YAML file called my-namespace.yaml
![image](https://user-images.githubusercontent.com/103019032/164191733-c4a9557c-b445-432c-ae97-9a7178b0e20a.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164166403-cee4da97-9f8f-4d47-ab53-bdca92767a2c.png)
![image](https://user-images.githubusercontent.com/103019032/164166616-6c9dfa35-cc86-4fae-bf14-0b1cb3846811.png)
- #### Another way to create namespace using othercommand.It can only file name not extension
![image](https://user-images.githubusercontent.com/103019032/164197366-71a6f1a9-934b-4735-82e8-7ff0643ca2e9.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164197676-45502de7-3d70-4ea9-809c-5daed01a1df3.png)
![image](https://user-images.githubusercontent.com/103019032/164197788-ee1713f3-a072-4e43-baaa-ffa17cb180f9.png)
- #### Delete a namespace with following command
![image](https://user-images.githubusercontent.com/103019032/164198189-5bdd01cb-03c8-47ff-b809-6cadf47aa7e1.png)
## *Pods in kubernetes*
- #### Single container pod :they can be simply created with the kubctl run command, where you have a defined image on the Docker registry which we will pull while creating a pod
![image](https://user-images.githubusercontent.com/103019032/164209319-c231f254-b46f-4143-a2b5-51b2ac995c66.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164211536-8f7da695-af4a-455e-aa7a-a2a9c2623f4d.png)
- #### Multi container pods are created using yaml with the definition of the containers
![image](https://user-images.githubusercontent.com/103019032/164372798-33f05adc-2033-4af7-88f1-bc21a863331d.png)
- #### Edit using nano editor with the contents
![image](https://user-images.githubusercontent.com/103019032/164372894-a585d31b-602e-4c69-9343-8bb3443e4c9c.png)
## *Implementation of storage class and PVC*
- #### Create a storage class using nano editor
![image](https://user-images.githubusercontent.com/103019032/164388514-0cf941a1-332c-4976-bff2-c4af4180c4bb.png)
- #### Create a storage class using kubectl create command
![image](https://user-images.githubusercontent.com/103019032/164388868-b4ff4f7b-e35c-4e88-8c83-8bf374acd85c.png)
- #### After that we create PVC using nano editor
![image](https://user-images.githubusercontent.com/103019032/164390786-77bbeaf4-f54a-4582-9fd6-ba07aa0af78d.png)
- #### Create a PVC using kubectl create command
![image](https://user-images.githubusercontent.com/103019032/164389097-d1435234-0cdc-45a9-a710-60e098b985b8.png)
- #### Show list of all pvc
![image](https://user-images.githubusercontent.com/103019032/164391129-3e943429-a097-4ebc-8659-0076e7b94e35.png)
## *Daemonset in kubernetes*
-#### Create a DaemonSet,You can describe a DaemonSet in a YAML file
![image](https://user-images.githubusercontent.com/103019032/164427312-2c6cced3-1ff7-434a-b2c9-ace7aae9a9a0.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164427745-0f53d700-e3a7-483c-a52e-5c57a6494189.png)
 #### * Implementation of Configmap and secret application (with DB) *
- #### we will create a simple YAML that contains the data
![image](https://user-images.githubusercontent.com/103019032/164449175-d58666a7-4eaa-4233-8118-6f607bbd0e44.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164449737-d78de4fb-8ba3-4c58-aa7e-c5510d12d9fe.png)
- #### These YAML and configmap can be created using the kubectl apply command 
![image](https://user-images.githubusercontent.com/103019032/164450691-9f79c936-5619-4f49-b86d-0a15c7a0bc0b.png)
- #### Use the following command with the appropriate ConfigMap name defined in the metadata section
![image](https://user-images.githubusercontent.com/103019032/164451291-64145f62-b279-4475-be52-e1c0762ef10c.png)
- #### we will create a simple YAML that contains the data
![image](https://user-images.githubusercontent.com/103019032/164452799-8dffb51c-5322-4d5a-b2a2-a0ac02971c59.png)
- #### Edit using nano editor with the contents:
![image](https://user-images.githubusercontent.com/103019032/164452077-e1ecfeb0-4bfa-40b2-9dfc-60d06daf137a.png)
- #### These YAML and secret can be created using the kubectl apply command
![image](https://user-images.githubusercontent.com/103019032/164452574-db9f8ebb-54b1-422c-8b33-eddfc61fc15f.png)
- #### Use the following command with the appropriate Service name defined in the metadata section
![image](https://user-images.githubusercontent.com/103019032/164453105-34e230f5-8adb-4683-8585-bd3d773afc74.png)
