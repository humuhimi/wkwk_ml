# wkwk_ml
try machine learning wkwk series

実行環境
EC2 Ubuntu Server 16.04 LTS (HVM), SSD Volume Type 
セキュリティグループ
HTTP TCP 80/カスタム TCP ルールTCP 8000 / SSH TCP 22 /カスタム TCP ルールTCP5000/HTTPS TCP 443
環境構築
sudo apt-get update
sudo apt install python-pip python3-pip
sudo pip install --upgrade
sudo add-apt-repository ppa:jonathonf/python-3.6
sudo apt-get update
python3 -m pip install numpy pandas sklearn jupyter flask 
jupyter notebook --generate-config
vi /root/.jupyter/jupyter_notebook_config.py

-(jupyter_notebook_config.py)-
c.NotebookApp.ip = '0.0.0.0'
c.NotebookApp.port = 8000
-

