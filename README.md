# linux_PR5
Директория включает в себя 3 файла: app.py, Dockerfile, requirements.txt
Выполняю команды:
docker build -t test_app .
docker run -d -p 5000:5000 test_app
docker ps 
Вывод терминала:
18b94176f928   test_app   "python app.py"   25 minutes ago   Up 25 minutes   0.0.0.0:5000->5000/tcp, :::5000->5000/tcp   zealous_pike
Проверка 
curl http://localhost:5000/hello/misha
Вывод
{"message":"Hello from Vasya, misha!"}
Программа работает корректно
