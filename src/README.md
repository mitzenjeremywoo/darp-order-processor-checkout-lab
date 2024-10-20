

cd checkout
docker buildx build . -t checkout:1.0.0

cd order-processor
docker buildx build . -t  order-processor:1.0.0


To run locally 

dapr run -f .
