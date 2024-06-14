# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
<a rel="me" href="https://hachyderm.io/@Searge">![@Searge@hachyderm.io](https://img.shields.io/badge/-@Searge-%232B90D9?logo=mastodon&logoColor=white)</a>

```python
# %%
"""Creating a class for keeping track of knowledge."""
import json
from dataclasses import asdict, make_dataclass

from rich import print

person = make_dataclass(
    "Person",
    [
        ("nick", str),
        ("name", str),
        ("pipelines", list[str]),
        ("web_services", list[str]),
        ("languages", list[str]),
        ("databases", list[str]),
        ("misc", list[str]),
        ("ongoing", list[str]),
    ],
    namespace={"to_json": lambda self: json.dumps(asdict(self), indent=4)},
)

# %%
# @title Initializing classes and creating lists
if __name__ == "__main__":
    pipelines    = ['GitLab Ci', 'GitHub Actions', 'AWS CodePipeline', 'Jenkins']
    web_services = ['nginx', 'apache', 'varnish', 'fastly', 'elastic', 'solr']
    languages    = ['YAML', 'Bash', 'Python', 'JS', 'Web']
    databases    = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc         = ['Ansible', 'Linux', 'LXC', 'Docker', 'Terraform', 'AWS']
    ongoing      = ['LPIC', 'Full Stack Web', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                pipelines, web_services, languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```

<sub>Thanks @rednafi for idea of script :wink:</sub>

### Statistics

[Skyline for 2021](https://skyline.github.com/Searge/2021)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) 
<!--START_SECTION:waka-->
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C585%20hrs%208%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1502 commits        ██████░░░░░░░░░░░░░░░░░░░   24.13 % 
🌆 Daytime                2700 commits        ███████████░░░░░░░░░░░░░░   43.38 % 
🌃 Evening                1783 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   907 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.57 % 
Tuesday                  850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Wednesday                789 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.68 % 
Thursday                 830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.03 % 
Sunday                   1024 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 31 mins       █████████████████░░░░░░░░   67.22 % 
Bash                     1 hr 29 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.51 % 
YAML                     58 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.84 % 
XML                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.17 % 
Other                    26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.13 % 

🔥 Editors: 
Zsh                      9 hrs 31 mins       █████████████████░░░░░░░░   67.22 % 
VS Code                  3 hrs 43 mins       ███████░░░░░░░░░░░░░░░░░░   26.30 % 
Vim                      43 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.16 % 
Obsidian                 11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.32 % 

💻 Operating System: 
Linux                    14 hrs 10 mins      █████████████████████████   100.00 % 
```


 Last Updated on 14/06/2024 00:41:51 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
