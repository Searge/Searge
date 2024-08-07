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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C699%20hrs%2013%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1578 commits        ██████░░░░░░░░░░░░░░░░░░░   24.39 % 
🌆 Daytime                2816 commits        ███████████░░░░░░░░░░░░░░   43.52 % 
🌃 Evening                1836 commits        ███████░░░░░░░░░░░░░░░░░░   28.37 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.10 % 
Tuesday                  910 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.06 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.36 % 
Thursday                 859 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Friday                   846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.53 % 
Sunday                   1074 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.60 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 15 mins       ████████████████░░░░░░░░░   62.27 % 
YAML                     3 hrs 44 mins       ███████░░░░░░░░░░░░░░░░░░   28.24 % 
Other                    32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.09 % 
Markdown                 24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.13 % 
CSS                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.87 % 

🔥 Editors: 
Zsh                      8 hrs 15 mins       ████████████████░░░░░░░░░   62.27 % 
VS Code                  4 hrs 24 mins       ████████░░░░░░░░░░░░░░░░░   33.25 % 
Obsidian                 24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.09 % 
Vim                      11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.39 % 

💻 Operating System: 
Linux                    13 hrs 16 mins      █████████████████████████   100.00 % 
```


 Last Updated on 07/08/2024 00:45:57 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
