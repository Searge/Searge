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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C570%20hrs%2047%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1497 commits        ██████░░░░░░░░░░░░░░░░░░░   24.09 % 
🌆 Daytime                2698 commits        ███████████░░░░░░░░░░░░░░   43.42 % 
🌃 Evening                1782 commits        ███████░░░░░░░░░░░░░░░░░░   28.68 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   906 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.58 % 
Tuesday                  846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.61 % 
Wednesday                789 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.70 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.32 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Saturday                 997 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.04 % 
Sunday                   1022 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 9 mins       ████████████░░░░░░░░░░░░░   48.65 % 
YAML                     8 hrs 33 mins       █████████░░░░░░░░░░░░░░░░   37.34 % 
Markdown                 1 hr 59 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.67 % 
Other                    21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.54 % 
INI                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.76 % 

🔥 Editors: 
Zsh                      11 hrs 9 mins       ████████████░░░░░░░░░░░░░   48.65 % 
VS Code                  9 hrs 52 mins       ███████████░░░░░░░░░░░░░░   43.06 % 
Obsidian                 1 hr 35 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.97 % 
Vim                      17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.31 % 
Unknown Editor           0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    22 hrs 55 mins      █████████████████████████   100.00 % 
```


 Last Updated on 07/06/2024 00:40:03 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
