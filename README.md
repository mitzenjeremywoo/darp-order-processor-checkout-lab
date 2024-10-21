
Clone the repository then go into the src folder.

Run the following command to build your image. 
cd order-processor
docker buildx build . -t  docker-account/order-processor:1.0.0
docker push

* cd checkout *
* docker buildx build . -t  docker-account/checkout:1.0.0  *
* docker push *

To deploy to your kubernetes cluster, run the following command

* kubectl apply -f root-folder/deploy/app/order-processor.yaml *

You will see there's 2 containers in the order-processor pod

* kubectl apply -f root-folder/deploy/app/checkout.yaml *
