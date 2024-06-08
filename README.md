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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C575%20hrs%2038%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1519 commits        ██████░░░░░░░░░░░░░░░░░░░   24.13 % 
🌆 Daytime                2712 commits        ███████████░░░░░░░░░░░░░░   43.09 % 
🌃 Evening                1822 commits        ███████░░░░░░░░░░░░░░░░░░   28.95 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   913 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.51 % 
Tuesday                  848 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.47 % 
Wednesday                795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.63 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Friday                   827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.14 % 
Saturday                 1034 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.43 % 
Sunday                   1049 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       13 hrs 59 mins      ███████████████░░░░░░░░░░   58.80 % 
YAML                     6 hrs 45 mins       ███████░░░░░░░░░░░░░░░░░░   28.41 % 
Markdown                 1 hr 44 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.31 % 
Other                    33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.35 % 
INI                      18 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.29 % 

🔥 Editors: 
Zsh                      13 hrs 59 mins      ███████████████░░░░░░░░░░   58.80 % 
VS Code                  7 hrs 57 mins       ████████░░░░░░░░░░░░░░░░░   33.40 % 
Obsidian                 1 hr 20 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.67 % 
Vim                      30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.11 % 
Unknown Editor           0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    23 hrs 48 mins      █████████████████████████   100.00 % 
```


 Last Updated on 08/06/2024 00:40:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
