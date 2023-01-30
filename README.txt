KURULUM

pip install -r requirements.txt




ÖRNEK BAŞLATMA KOMUTU

sudo python main.py [INTERFACE NAME] [RULE FILE PATH]



SENDER ÖRNEK BAŞLATMA KOMUDU

sudo python sender.py x [RULE FILE PATH]

[!!] sender çalıştırılacağı zaman INTERFACE1 ve INTERFACE değişkenlerini 
ayarlamayı unutmayın INTERFACE1 netifaces kütüphanesinin kabul ettiği formatta
INTERFACE değişkeni scap kütüphanesinin istediği formatta olması gerekmektedir.

[!!] Uyarı program root yetkisi ile çalıştırılmadığında düzgün çalışmayabilir.




KURAL SYNTAX

PROTO [!]IP|any:[!]PORT(RANGE)|any <>|-> [!]IP|any:[!]PORT(RANGE)|any *PAYLOAD

Örnek
ICMP 192.168.178.22:any -> 1.1.1.1:[500-510] * # -IDS
