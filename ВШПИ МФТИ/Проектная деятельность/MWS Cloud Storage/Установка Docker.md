##### 1. Установка Docker + Docker compose plugin
**Windows**
https://www.docker.com/products/docker-desktop/
**Важно**: Отметьте "Use WSL 2 instead of Hyper-V" (рекомендуется)

**Linux (Ubuntu/Debian)**
sudo apt-get update
sudo apt-get install docker.io

sudo curl -L "https://github.com/docker/compose/releases/latest/download/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose

##### 2. (Опционально) Установка плагина Docker в IDEA
##### 3. Создание конфигураций в IDEA

![[Pasted image 20251102190514.png]]
Нажимаем на:
1. Текущую конфигурацию (Слева от кнопки запуска)
2. Edit configurations
3. Плюсик 
4. Docker $\to$ Dockerfile
5. В "Image tag" вводим "cloud-storage-app"
6. Плюсик
7. Docker $\to$ Docker compose
8. В "Compose files" вводим "./docker-compose.yml; "
9. В "Services" вводим "app, postgres,"

##### 4. Запуск сервисов

1. После изменения кода или pom.xml выбираем конфиг "Docker" и запускаем его (Shift+F10)
2. Для запуска сервисов (оркестрации) выбираем конфиг "Docker compose" и запускаем его (Shift+F10)