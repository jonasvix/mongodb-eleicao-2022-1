# mongodb-eleicao-2022-1
Arquivo exportado de um banco mongodb, com os dados das eleições 2022 - 1º turno

## Precisa instalar:
    MongoDB: 6

Esse banco mongodb foi gerado pela aplicação:
https://github.com/jonasvix/import-eleicao-2022


Esse arquivo "eleicao2022.01.gz" mongodb foi gerado usando o comando:
> mongodump --archive=eleicao2022.01.gz --gzip --db=eleicao2022
    - Detalhes: https://www.mongodb.com/docs/database-tools/mongodump/#compress-the-output

Para importar esse arquivo, use o comando abaixo, e assim vai criar o seu banco mongodb:
> mongorestore --archive=eleicao2022.01.gz --gzip --nsFrom="eleicao2022.*" --nsTo="eleicao2022.*"
    - Detalhes: https://www.mongodb.com/docs/database-tools/mongorestore/#restore-from-compressed-data


Pasta com backup do arquivo "eleicao2022.01.gz":
https://www.dropbox.com/sh/kygi5wo789vvmm9/AAAgH28WHh1QJAoPToStiQEKa?dl=0


Arquivo backup "eleicao2022.01.gz":
https://www.dropbox.com/s/69oyvwxxmkb8tt3/eleicao2022.01.gz?dl=0
