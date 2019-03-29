# wkwk_ml
try machine learning wkwk series

実行環境<br>
-EC2 Ubuntu Server 16.04 LTS (HVM), SSD Volume Type <br>
セキュリティグループ
HTTP TCP 80/カスタム TCP ルールTCP 8000 / SSH TCP 22 /カスタム TCP ルールTCP5000/HTTPS TCP 443
環境構築<br>
-sudo apt-get update
-sudo apt install python-pip python3-pip<br>
sudo pip install --upgrade<br>
sudo add-apt-repository ppa:jonathonf/python-3.6<br>
sudo apt-get update<br>
python3 -m pip install numpy pandas sklearn jupyter flask <br>
jupyter notebook --generate-config<br>
vi /root/.jupyter/jupyter_notebook_config.py<br>

-(jupyter_notebook_config.py)-<br>
c.NotebookApp.ip = '0.0.0.0'<br>
c.NotebookApp.port = 8000<br>

