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
# Update the apt package index and install packages to allow apt to use a repository over HTTPS
```bash
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
```
### Добавляем GPG key
```bash
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```
### Настраиваем Репозиторий
```bash
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/debian \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
### Update the apt package index
sudo apt-get update

