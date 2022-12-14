Build an Image
docker build -t nishantpani55/blockchain_21194530:smartcontract .

Run an image
docker run -p 8090:8080 --name x21194530 -d nishantpani55/blockchain_21194530:smartcontract

Run the curl command
This transfers ETH:

curl --header "Content-Type: application/json" --request POST --data '{"address":"0x42442147D273EaC997EA77217C9E5C170434FF7D","amount":"0.005"}' http://localhost:8090/eth

This transfers token:

curl --header "Content-Type: application/json" --request POST --data '{"address":"0x42442147D273EaC997EA77217C9E5C170434FF7D"}' http://localhost:8090/token
