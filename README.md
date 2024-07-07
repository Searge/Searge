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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C645%20hrs%2025%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1940 commits        ██████░░░░░░░░░░░░░░░░░░░   25.12 % 
🌆 Daytime                3083 commits        ██████████░░░░░░░░░░░░░░░   39.92 % 
🌃 Evening                2410 commits        ████████░░░░░░░░░░░░░░░░░   31.21 % 
🌙 Night                  289 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1074 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.91 % 
Tuesday                  949 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.29 % 
Wednesday                933 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.08 % 
Thursday                 882 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.42 % 
Friday                   867 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.23 % 
Saturday                 1506 commits        █████░░░░░░░░░░░░░░░░░░░░   19.50 % 
Sunday                   1511 commits        █████░░░░░░░░░░░░░░░░░░░░   19.57 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 50 mins       ███████████████░░░░░░░░░░   61.02 % 
YAML                     3 hrs 12 mins       ██████░░░░░░░░░░░░░░░░░░░   22.14 % 
Markdown                 1 hr 31 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.49 % 
SSH Config               18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.18 % 
Diff                     12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.39 % 

🔥 Editors: 
Zsh                      8 hrs 50 mins       ███████████████░░░░░░░░░░   61.02 % 
VS Code                  4 hrs 22 mins       ████████░░░░░░░░░░░░░░░░░   30.26 % 
Obsidian                 1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.13 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.59 % 

💻 Operating System: 
Linux                    14 hrs 28 mins      █████████████████████████   100.00 % 
```


 Last Updated on 07/07/2024 00:44:12 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
