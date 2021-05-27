# Minecraft
mod for server 
https://www.curseforge.com/minecraft/mc-mods/entityculling

mod not sure
1. https://www.curseforge.com/minecraft/mc-mods/macaws-fences-and-walls#comments
2. https://www.curseforge.com/minecraft/mc-mods/diagonal-fences
3. https://www.curseforge.com/minecraft/mc-mods/majos-broom
4. https://www.curseforge.com/minecraft/mc-mods/rule-control-rc
5. https://www.curseforge.com/minecraft/mc-mods/physics-mod/files
6. https://www.curseforge.com/minecraft/mc-mods/when-dungeons-arise
7. https://www.curseforge.com/minecraft/mc-mods/tablechair?__cf_chl_jschl_tk__=fb9fd3bb524a16d3170ca1b0ef4285997106a2ed-1622003642-0-AUhcGVeUDskdP0AhH5rgkf8Fcl1_KQJh7jXgtxc0nCdxL9GDEwqWSvCjuAxBbmZzjZyEhx28AoehDsq0PCDwE2GH4TuHEemUpV9eDQlTNMYJUGzVin3GjqBMiga-RCVluHOEKT9Ozv3LJQNZurykDywrLUFgB4EbT6ci5tWA2QDaJre_Dp3_X934R_mxi0STlHJAPAcmOSvtWXUMq8unxiJ6P-AGR-2IRNqEn-XVBoqfbBLkDCsKv4x13c3ee8L8FzKeFfDnbJPMJWAs-CqGIKxzf63Hvvq8q7YgXgyaI5UHIux3mAVXKNrILvP90cizHH_xoqeX3eiDpBL6AMbbxCPTG-Q9jxIsg349fXG-H85Yt6AkXeJEAcYniuyVcmK1FRAK9iNMJI5N7mc-y6VnIHEML7LM43dE8yIQ960GXWt7Aa2uFQlcXtsMJ08XY8SmznAmwFd9rwuby48JwlLi3bNLMUujwA-4fZudXruUGY77npX5uqtw7kgXJyNJE6ZowA
8. https://www.curseforge.com/minecraft/mc-mods/callable-horses/files
9. https://www.curseforge.com/minecraft/mc-mods/anthill-inside

mod need time
1. https://www.curseforge.com/minecraft/mc-mods/refined-storage





python code 
import requests as req
import subprocess,zipfile,os,shutil
from tqdm import tqdm

url = 'https://github.com/vic0706/Minecraft/archive/refs/heads/main.zip'
def download(url):
    filename = url.split('/')[-1]
    r = req.get(url, stream=True)
    with open(filename, 'wb') as f:
        for data in tqdm(r.iter_content(1024)):
            f.write(data)
    return filename

def zip(file):
	unzip = zipfile.ZipFile(file, 'r')
	unzip.extractall()
	unzip.close()


shutil


#download(url)
#zip('main.zip')



#subprocess.call(['java', '-jar', 'forge-1.16.5-36.1.0-installer.jar'])


