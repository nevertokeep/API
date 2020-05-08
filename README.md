# API
import requests

url = "https://beta-api-v2.chuangkit.com//template/user/favorite/unCollect.do?_dataType=json&ids=154455&nFid=0"

payload = {}
headers = {
  'COOKIE': 'Sec_User_id=1373403;SEC_SESSION=462F53DE94AD8EF04B3832F8AA5ED549'
}

response = requests.request("POST", url, headers=headers, data = payload)

print(response.text.encode('utf8'))
