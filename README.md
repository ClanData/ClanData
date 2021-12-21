import time as mm
import sys as n
import requests
import random
from colorama import *
g = Fore.GREEN
r = Fore.RED
y = Fore.YELLOW
c = Fore.CYAN
def slow(M):
	for c in M + '\n':
		n.stdout.write(c)
		n.stdout.flush()
		mm.sleep(0.60/ 120)
by = "EntrBot"
slow(f'''{Fore.YELLOW}
The tool is running..
''')

def slow(M):
	for c in M + '\n':
		n.stdout.write(c)
		n.stdout.flush()
		mm.sleep(0.60/ 120)
by = "EntrBot"
slow(f'''{Fore.YELLOW}
================================================
''')
def slow(M):
	for c in M + '\n':
		n.stdout.write(c)
		n.stdout.flush()
		mm.sleep(0.60/ 120)
by = "EntrBot"
slow(f'''{Fore.YELLOW}

 _____   _   _   _____   ____    ____     ___    _____ 
| ____| | \ | | |_   _| |  _ \  | __ )   / _ \  |_   _|
|  _|   |  \| |   | |   | |_) | |  _ \  | | | |   | |  
| |___  | |\  |   | |   |  _ <  | |_) | | |_| |   | |  
|_____| |_| \_|   |_|   |_| \_\ |____/   \___/    |_|  
                                                       
''')
def slow(M):
	for c in M + '\n':
		n.stdout.write(c)
		n.stdout.flush()
		mm.sleep(0.60/ 120)
by = "EntrBot"
slow(f'''{Fore.YELLOW}
================================================

''')

rt = requests.session()
litters = 'qwertyuiopasdfghjklzxcvbnm1234567890'
u = ''

id = input("Enter Id :")

token = input(" Enter Bot Token : ")
print('')

hea = {
        'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
        'accept-encoding': 'gzip, deflate, br',
        'accept-language': 'en-US,en;q=0.9,ar;q=0.8',
        'cache-control': 'max-age=0',
        'sec-ch-ua': '" Not;A Brand";v="99", "Google Chrome";v="91", "Chromium";v="91"',
        'sec-ch-ua-mobile': '?0',
        'sec-fetch-dest': 'document',
        'sec-fetch-mode': 'navigate',
        'sec-fetch-site': 'same-origin',
        'sec-fetch-user': '?1',
        'upgrade-insecure-requests': '1',
        'user-agent': 'Mozilla/5.0(Windows NT 10.0;Win64;x64) AppleWebKit/537.36(KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36'
    }
while True:
 user = str("".join(random.choice(litters)for x in range(0)))
 user1 = str("".join(random.choice(litters)for x in range(4)))
 usernames = user + u + user1
 tiko = f'https://www.tiktok.com/@{usernames}?'
 reqsnd = rt.get(tiko, headers=hea).status_code
 if reqsnd == 404:
         print(g + f' [+] {usernames} متاح او مبند ')
         bot = f"https://api.telegram.org/bot{token}/sendMessage?chat_id={id}&text=متاح او مبند : {usernames}\n𝘽𝙔 : @aaqx7"
         rt.get(bot)
 else:
   print(r + f' [+] {usernames} غير متاح ')
