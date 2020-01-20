# ssh to container with bash
docker exec -it flask_hello_docker_flask_1 bash 

# execute py script
docker exec -it flask_hello_docker_flask_1 python train_model.py

# curl post json
curl --header "Content-Type: application/json" \
  --request POST \
  --data '{"flower":"1,2,3,7"}' \
  http://localhost:5000/iris_post