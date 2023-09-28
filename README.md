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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C238%20hrs%2025%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1362 commits        ██████░░░░░░░░░░░░░░░░░░░   22.62 % 
🌆 Daytime                2714 commits        ███████████░░░░░░░░░░░░░░   45.07 % 
🌃 Evening                1725 commits        ███████░░░░░░░░░░░░░░░░░░   28.64 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.67 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   849 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.10 % 
Tuesday                  775 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.87 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Thursday                 851 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.55 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.39 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     2 hrs 35 mins       ███████░░░░░░░░░░░░░░░░░░   27.37 % 
Markdown                 2 hrs 24 mins       ██████░░░░░░░░░░░░░░░░░░░   25.36 % 
Bash                     1 hr 52 mins        █████░░░░░░░░░░░░░░░░░░░░   19.82 % 
Go                       1 hr 23 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Ezhil                    28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.04 % 

🔥 Editors: 
VS Code                  7 hrs 28 mins       ████████████████████░░░░░   78.70 % 
Obsidian                 1 hr 55 mins        █████░░░░░░░░░░░░░░░░░░░░   20.20 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.10 % 

💻 Operating System: 
Linux                    9 hrs 25 mins       █████████████████████████   99.28 % 
Windows                  4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.72 % 
```


 Last Updated on 28/09/2023 00:09:28 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
