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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C133%20hrs%205%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1218 commits        ██████░░░░░░░░░░░░░░░░░░░   22.23 % 
🌆 Daytime                2465 commits        ███████████░░░░░░░░░░░░░░   45.00 % 
🌃 Evening                1585 commits        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   783 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.26 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.33 % 
Saturday                 849 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   833 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 8 hrs 38 mins       █████████░░░░░░░░░░░░░░░░   34.64 % 
YAML                     8 hrs 2 mins        ████████░░░░░░░░░░░░░░░░░   32.23 % 
Bash                     3 hrs 59 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.04 % 
Other                    1 hr 7 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.54 % 
Makefile                 42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.83 % 

🔥 Editors: 
VS Code                  17 hrs 3 mins       █████████████████░░░░░░░░   68.38 % 
Obsidian                 7 hrs 51 mins       ████████░░░░░░░░░░░░░░░░░   31.53 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.09 % 

💻 Operating System: 
Linux                    24 hrs 56 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/07/2023 00:10:36 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
