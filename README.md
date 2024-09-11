# ml-1 


### 1. Обновляем список доступных пакетов, обновлений

```bash
sudo apt-get update
```
### 2. Скачиваем Анаконду

```bash
wget https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh
bash Anaconda3-2022.05-Linux-x86_64.s
```
### 3. Устанавливаем Docker и Docker Compose
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
