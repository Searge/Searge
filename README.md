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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C469%20hrs%2058%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1521 commits        ██████░░░░░░░░░░░░░░░░░░░   24.25 % 
🌆 Daytime                2712 commits        ███████████░░░░░░░░░░░░░░   43.23 % 
🌃 Evening                1791 commits        ███████░░░░░░░░░░░░░░░░░░   28.55 % 
🌙 Night                  249 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.97 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   896 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.28 % 
Tuesday                  813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.96 % 
Wednesday                836 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.33 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.60 % 
Saturday                 1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.96 % 
Sunday                   1034 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 29 mins       ██████████████░░░░░░░░░░░   57.57 % 
Markdown                 2 hrs 36 mins       █████░░░░░░░░░░░░░░░░░░░░   20.03 % 
sh                       1 hr 32 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.78 % 
Bash                     25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.30 % 
Other                    15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.02 % 

🔥 Editors: 
VS Code                  8 hrs 48 mins       █████████████████░░░░░░░░   67.56 % 
Obsidian                 1 hr 37 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.51 % 
Zsh                      1 hr 32 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.78 % 
Vim                      1 hr 3 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.14 % 

💻 Operating System: 
Linux                    13 hrs 1 min        █████████████████████████   100.00 % 
```


 Last Updated on 07/05/2024 00:40:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
