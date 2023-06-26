# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## An DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C093%20hrs%2034%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1210 commits        ██████░░░░░░░░░░░░░░░░░░░   22.06 % 
🌆 Daytime                2457 commits        ███████████░░░░░░░░░░░░░░   44.79 % 
🌃 Evening                1608 commits        ███████░░░░░░░░░░░░░░░░░░   29.32 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   791 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.42 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Wednesday                716 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.24 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.31 % 
Saturday                 860 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.68 % 
Sunday                   823 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.00 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 11 hrs 27 mins      ███████████████░░░░░░░░░░   61.17 % 
YAML                     2 hrs 20 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.49 % 
INI                      2 hrs 20 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.49 % 
Other                    55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.93 % 
Bash                     40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.58 % 

🔥 Editors: 
VS Code                  9 hrs 31 mins       █████████████░░░░░░░░░░░░   50.90 % 
Obsidian                 8 hrs 39 mins       ████████████░░░░░░░░░░░░░   46.27 % 
Vim                      31 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.83 % 

💻 Operating System: 
Linux                    18 hrs 24 mins      █████████████████████████   98.38 % 
Mac                      18 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.62 % 
```


 Last Updated on 26/06/2023 00:10:44 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
