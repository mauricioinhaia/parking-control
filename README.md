# Parking Spot
# 🚧 Sobre o Projeto

Refere-se a uma API de controle de estacionamento, podendo ser aplicado em condomínios para gerenciar as vagas.
Vinculando as mesmas aos responsáveis, placa do veículo, apartamento e bloco.

# 📋 Requisitos

- Java (JDK 17)
- PostgreSQL (DB parking-control)

# 🖧 EndPoints
Podem ser importados no Postman através do arquivo ParkingSpot.postman_collection disponibilizado nesse projeto.
#### GET All Parking Spots
```
http://localhost:8080/parking-spot
```
#### GET Parking Spot by ID
```
http://localhost:8080/parking-spot/05e14dd4-df31-4a98-9eac-d42270947dcd
```
#### POST Parking Spot
```
http://localhost:8080/parking-spot

#Body:
{
    "parkingSpotNumber": "4A",
    "licensePlateCar": "MJT5675",
    "brandCar": "Volkswagen",
    "modelCar": "Fox",
    "colorCar": "Vermelho",
    "responsibleName": "Arthur Inhaia",
    "apartment": "202",
    "block": "A"
}
```
#### PUT Parking Spot
```
http://localhost:8080/parking-spot/05e14dd4-df31-4a98-9eac-d42270947dcd

#Body:
{
    "parkingSpotNumber": "4A",
    "licensePlateCar": "MCQ0899",
    "brandCar": "Chevrolet",
    "modelCar": "Cruze",
    "colorCar": "Azul",
    "responsibleName": "Arthur Inhaia",
    "apartment": "202",
    "block": "A"
}
```
#### DELETE Parking Spot
```
http://localhost:8080/parking-spot/05e14dd4-df31-4a98-9eac-d42270947dcd
```

# 💻 Como executar o Projeto
```
# Criar uma pasta para salvar o projeto
mkdir /home/seunomeusuario/git

# Acessar a pasta para salvar
cd /home/seunomeusuario/git

# Clonar repositório
git clone https://github.com/mauricioinhaia/parking-control.git

# Acessar pasta para executar
cd parking-control/

# Executar o Projeto
./mvnw spring-boot:run
```

# Autor
[Mauricio Inhaia](https://www.linkedin.com/feed/ "LinkedIn")