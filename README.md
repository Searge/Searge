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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C840%20hrs%2053%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1648 commits        ██████░░░░░░░░░░░░░░░░░░░   25.23 % 
🌆 Daytime                2794 commits        ███████████░░░░░░░░░░░░░░   42.78 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.19 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   944 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.45 % 
Tuesday                  896 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.72 % 
Wednesday                853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.06 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.53 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 6 mins        ███████████░░░░░░░░░░░░░░   44.14 % 
YAML                     8 hrs 3 mins        ███████████░░░░░░░░░░░░░░   43.92 % 
DNS Zone                 55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.00 % 
Other                    35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.19 % 
Markdown                 29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.70 % 

🔥 Editors: 
VS Code                  9 hrs 28 mins       █████████████░░░░░░░░░░░░   51.61 % 
Zsh                      8 hrs 6 mins        ███████████░░░░░░░░░░░░░░   44.14 % 
Obsidian                 29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.64 % 
Vim                      17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.61 % 

💻 Operating System: 
Linux                    18 hrs 21 mins      █████████████████████████   100.00 % 
```


 Last Updated on 16/10/2024 00:51:41 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
