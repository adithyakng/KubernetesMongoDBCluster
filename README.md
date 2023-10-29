This yaml files create a mongodb-express server and connects it with mongodb
Total we have created the following
1) MongoDB Deployment
2) MongoExpress Deployment
3) MongoDB service 
4) mongo-express-service
5) Mong0-secret for storing db name and password
6) Mongo-configmap for storing the db url


Order:
kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo-configmap.yaml
kubectl apply -f monogo.yaml
kubectl apply -f monogo-express.yaml