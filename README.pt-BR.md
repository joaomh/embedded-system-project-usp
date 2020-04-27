# Reconhecimento de Veículos 

## Sumário

- [Descrição](#Descrição)
- [Requisitos](#Requisitos)
- [Tecnologia](#Tecnologias)
- [Desenvolvedores](#Desenvolvedores)

## Descrição
Este projeto foca no desenvolvimento de um sistema embarcado para o reconhecimento de veículos e suas placas

![Exemplo](./assets/vehicle_ex.jpeg)

## Requisitos

### Requisitos funcionais
 O sistema deve identificar o carro do condômino e abrir o portão para ele
- Procurar classe "carro" na imagem gerada pelo sensor câmera
- Procurar classe "placa" no objeto "carro" e comparar com banco de dados de "placas de carros de condôminos"
- Se constar no banco de dados, acionar atuador "portão da garagem"
- Fechar depois de um tempo

[Opcional, para caso se queira fazer algo mais robusto e completo]


 O sistema deve ter uma interface que permita ler autorizações para entrada de carros de visitantes (vulgo "condômino gera QR code para o visitante, ele põe no scanner do interfone, e abre o portão caso o QR bata com o QR autorizado" ou "a câmera que checa as placas está quebrada, mas o condômino consegue mostrar QR dele e abrir o portão")

### Requisitos não funcionais
- O sistema deve responder a 90% das checagens em menos de 5 segundos (ou qualquer número arbitrário)
- O sistema deve autorizar corretamente em 100% das vezes (é preferível que não reconheça uma placa autorizada e exija uma checagem secundária do que reconhecer uma placa não autorizada e deixar alguém indevido entrar)
- O sistema deve checar que o carro entrou e acionar o atuador do portão após 2 segundos da entrada

## Tecnologias
- Python

## Desenvolvedores
- [Eduardo Key Shiratori](https://github.com/EduardoKeyS)
- [Joao Pinheiro](https://github.com/joaomh)
- [Raphael Hideki](https://github.com/raphaelyokosawa/)
- [Reon Fujieda](https://github.com/reonfk)
