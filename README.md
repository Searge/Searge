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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C198%20hrs%2049%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1347 commits        ██████░░░░░░░░░░░░░░░░░░░   22.67 % 
🌆 Daytime                2678 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1697 commits        ███████░░░░░░░░░░░░░░░░░░   28.55 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   836 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  766 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Wednesday                793 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Thursday                 840 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.68 % 
Saturday                 918 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.45 % 
Sunday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.44 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 17 mins       ██████████░░░░░░░░░░░░░░░   40.40 % 
YAML                     2 hrs 52 mins       █████████░░░░░░░░░░░░░░░░   35.30 % 
Bash                     1 hr 26 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.75 % 
Blade Template           10 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.19 % 
Ezhil                    10 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.18 % 

🔥 Editors: 
VS Code                  4 hrs 56 mins       ███████████████░░░░░░░░░░   60.76 % 
Obsidian                 3 hrs 6 mins        ██████████░░░░░░░░░░░░░░░   38.34 % 
Zsh                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.40 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.31 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.19 % 

💻 Operating System: 
Linux                    8 hrs 7 mins        █████████████████████████   100.00 % 
```


 Last Updated on 06/09/2023 00:09:09 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
