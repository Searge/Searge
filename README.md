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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C156%20hrs%2031%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1214 commits        ██████░░░░░░░░░░░░░░░░░░░   22.44 % 
🌆 Daytime                2435 commits        ███████████░░░░░░░░░░░░░░   45.01 % 
🌃 Evening                1550 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  211 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.90 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   776 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
Tuesday                  726 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.42 % 
Wednesday                697 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Thursday                 767 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
Friday                   777 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.36 % 
Saturday                 843 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.58 % 
Sunday                   824 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.23 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 5 hrs 3 mins        █████████████░░░░░░░░░░░░   52.30 % 
YAML                     2 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   23.12 % 
Bash                     43 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.51 % 
Other                    41 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.20 % 
INI                      28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.86 % 

🔥 Editors: 
VS Code                  5 hrs 21 mins       ██████████████░░░░░░░░░░░   55.33 % 
Obsidian                 4 hrs 17 mins       ███████████░░░░░░░░░░░░░░   44.37 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.30 % 

💻 Operating System: 
Linux                    9 hrs 40 mins       █████████████████████████   100.00 % 
```


 Last Updated on 26/07/2023 00:09:32 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
