How to run:
* For Linux and Minikube or Mac OS and Minikube:
  1. **Open terminal**
  2. Navigate to the repository folder
  3. minikube start
  4. **eval $(minikube docker-env)**
  5. docker build -t spring .
  6. kubectl apply -f mysql.yaml,spring.yaml
  7. Wait for a couple of minutes
  8. minikube service spring
* For Windows and Minikube:
  1. **Run PowerShell as administrator**
  2. Navigate to the repository folder
  3. minikube start
  4. **minikube docker-env | Invoke-Expression**
  5. docker build -t spring .
  6. kubectl apply -f mysql.yaml,spring.yaml
  7. Wait for a couple of minutes
  8. minikube service spring