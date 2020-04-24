mvn test -Djitsi-meet.instance.url="https://meeting1.devopsviet.com"


mvn \
-Dorg.jitsi.malleus.conferences=20 \
-Dorg.jitsi.malleus.participants=20 \
-Dorg.jitsi.malleus.senders=20 \
-Dorg.jitsi.malleus.duration=6000 \
-Djitsi-meet.instance.url="https://meeting1.devopsviet.com" \
test



mvn test -Djitsi-meet.instance.url="https://meeting1.devopsviet.com" -Djitsi-meet.tests.toRun="MuteTest,TCPTest"

./scripts/malleus.sh --conferences=1 --participants=3 --senders=2 --audio-senders=1 --duration=300 --instance-url=https://meeting1.devopsviet.com

./scripts/malleus.sh --conferences=1 --participants=4 --senders=2 --audio-senders=2 --duration=30 --room-name-prefix=jitsihammertest --hub-url=https://jitsi.mydomain.tld


java -jar selenium-server-standalone.jar -role hub



http://10.10.10.87:4444/grid/console

java -jar selenium-server-standalone-3.141.59.jar -role hub


java -Dwebdriver.chrome.driver=path/to/chromedriver -jar selenium-server-standalone.jar -role node -maxSession 1 -hub http://yourip:4444/grid/register -browser browserName=chrome,version=80,platform=Linux,maxInstances=1

java -Dwebdriver.chrome.driver=/root/chromedriver -jar selenium-server-standalone-3.141.59.jar -role node -maxSession 1 -hub http://10.10.10.87:4444/grid/register -browser browserName=chrome,version=80,platform=Linux,maxInstances=1

java -Dwebdriver.chrome.driver=path/to/chromedriver -jar selenium-server-standalone.jar -role node -maxSession 1 -hub http://yourip:4444/grid/register -browser browserName=chrome,version=80,platform=Linux,maxInstances=1



./scripts/malleus.sh --conferences=2 --participants=4 --senders=1 --audio-senders=2 --duration=120 --room-name-prefix=hamertesting --hub-url=http://10.10.10.87:4444/wd/hub --instance-url=https://meeting1.devopsviet.com



docker run -d -p 4444:4444 --name selenium-hub selenium/hub:3.141.59-20200409


docker run -d -e HUB_HOST=10.10.10.87 -v /dev/shm:/dev/shm selenium/node-chrome:3.141.59-20200409


./scripts/malleus.sh --conferences=1 --participants=10 --senders=1 --audio-senders=2 --duration=120 --room-name-prefix=hamertesting --hub-url=http://10.10.10.87:4444/wd/hub --instance-url=https://meeting1.devopsviet.com













java -Dwebdriver.chrome.driver=/root/chromedriver -jar selenium-server-standalone-3.141.59.jar -role node -maxSession 1 -hub http://10.10.10.87:4444/grid/register -browser browserName=me,version=80.0.3987.106,platform=Linux,maxInstances=1 -host 10.10.10.87 -port 5555









./scripts/malleus.sh --conferences=1 --participants=30 --senders=10 --audio-senders=10 --duration=120 --room-name-prefix=hamertesting --hub-url=http://10.10.10.87:4444/wd/hub --instance-url=https://meeting1.devopsviet.com


/tmp/jitsi/file_example_WAV_1MG.wav


mvn test -Djitsi-meet.instance.url="https://meeting1.devopsviet.com"


mvn -Dthreadcount=1 -Dorg.jitsi.malleus.conferences=1 -Dorg.jitsi.malleus.participants=5 -Dorg.jitsi.malleus.senders=2 -Dorg.jitsi.malleus.duration=300 -Djitsi-meet.instance.url="https://meeting1.devopsviet.com" test


./scripts/malleus.sh --conferences=1 --participants=15 --senders=1 --audio-senders=2 --duration=120 --room-name-prefix=hamertesting --hub-url=http://10.10.10.87:4444/wd/hub --instance-url=https://meeting1.devopsviet.com


mvn \
-Dthreadcount=1 \
-Dorg.jitsi.malleus.conferences=1 \
-Dorg.jitsi.malleus.participants=10 \
-Dorg.jitsi.malleus.senders=5 \
-Dorg.jitsi.malleus.audio_senders=5 \
-Dorg.jitsi.malleus.duration=60 \
-Dorg.jitsi.malleus.room_name_prefix=hamertesting \
-Dremote.address=http://10.10.10.87:4444/wd/hub \
-Djitsi-meet.tests.toRun=MalleusJitsificus \
-Dwdm.gitHubTokenName=jitsi-jenkins \
-Dremote.resource.path=/root/jitsi-meet-torture \
-Djitsi-meet.instance.url=https://meeting1.devopsviet.com \
-Djitsi-meet.isRemote=true \
-Dchrome.disable.nosanbox=true \
test



mvn \
-Dthreadcount=1 \
-Dremote.address=http://10.10.10.87:4444/wd/hub \
-Djitsi-meet.tests.toRun=LipSyncTest \
-Dwdm.gitHubTokenName=jitsi-jenkins \
-Dremote.resource.path=/root/jitsi-meet-torture \
-Djitsi-meet.instance.url=https://meeting1.devopsviet.com \
-Djitsi-meet.isRemote=true \
-Dchrome.disable.nosanbox=true \
test

LipSyncTest


sudo apt-get update -y
sudo apt-get install -y gnupg curl wget unzip xvfb libxi6 libgconf-2-4 default-jdk
sudo curl -sS -o - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
sudo echo "deb [arch=amd64]  http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list
sudo apt-get -y update
sudo apt-get -y install google-chrome-stable
sudo apt-get install git -y && git clone https://github.com/lacoski/jitsi-meet-torture.git