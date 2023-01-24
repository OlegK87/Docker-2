Для сборки образа используем следующую комманду: docker build ./ --tag stockproducts
Для запуска контейнера используем следующую комманду: docker run --name my_stockproducts -d -p 8000:8000