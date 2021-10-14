# desafio1-rotten-potatoes
Nesse desafio rodamos 02 container um web outro de banco de dados usando o recurso do docker-compose

Principais pontos de atenção 
A - Declarar o volume para ter persistencia de dados do mongo
B - Declarar network com o driver correto e assim tem comunicação entre os 2 container
C - No services informar qual network e as váriaveis de ambiente que consegui pegar dentro do arquivo app.py para conexão com o mongo. Informar que o docker só pode iniciar após o pod do mongo subir para isso usamos a váriavel depends_on
D - No mondo não esquecer de informar o caminho do volume persistente