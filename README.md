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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C557%20hrs%207%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1491 commits        ██████░░░░░░░░░░░░░░░░░░░   24.08 % 
🌆 Daytime                2687 commits        ███████████░░░░░░░░░░░░░░   43.39 % 
🌃 Evening                1777 commits        ███████░░░░░░░░░░░░░░░░░░   28.70 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   899 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.52 % 
Tuesday                  838 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Wednesday                787 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.71 % 
Thursday                 823 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Saturday                 997 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.10 % 
Sunday                   1022 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.51 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     11 hrs 17 mins      ████████████░░░░░░░░░░░░░   48.59 % 
sh                       7 hrs 15 mins       ████████░░░░░░░░░░░░░░░░░   31.18 % 
Markdown                 2 hrs 9 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.29 % 
Bash                     1 hr 29 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.38 % 
Other                    22 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.58 % 

🔥 Editors: 
VS Code                  13 hrs 46 mins      ███████████████░░░░░░░░░░   59.26 % 
Zsh                      7 hrs 15 mins       ████████░░░░░░░░░░░░░░░░░   31.18 % 
Obsidian                 1 hr 58 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.47 % 
Vim                      15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.09 % 

💻 Operating System: 
Linux                    23 hrs 15 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/06/2024 00:39:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
