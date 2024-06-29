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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C625%20hrs%208%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1550 commits        ██████░░░░░░░░░░░░░░░░░░░   24.39 % 
🌆 Daytime                2732 commits        ███████████░░░░░░░░░░░░░░   42.98 % 
🌃 Evening                1831 commits        ███████░░░░░░░░░░░░░░░░░░   28.81 % 
🌙 Night                  243 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   926 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.57 % 
Tuesday                  870 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.69 % 
Wednesday                797 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.54 % 
Thursday                 835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.14 % 
Friday                   831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Saturday                 1045 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.44 % 
Sunday                   1052 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.55 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       15 hrs 41 mins      █████████████████░░░░░░░░   67.63 % 
YAML                     5 hrs 44 mins       ██████░░░░░░░░░░░░░░░░░░░   24.76 % 
Docker                   31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.24 % 
Bash                     26 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.90 % 
Other                    21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.52 % 

🔥 Editors: 
Zsh                      15 hrs 41 mins      █████████████████░░░░░░░░   67.63 % 
VS Code                  7 hrs 13 mins       ████████░░░░░░░░░░░░░░░░░   31.17 % 
Obsidian                 8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.63 % 
Vim                      7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.57 % 

💻 Operating System: 
Linux                    23 hrs 12 mins      █████████████████████████   100.00 % 
```


 Last Updated on 29/06/2024 00:40:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
