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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C645%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1553 commits        ██████░░░░░░░░░░░░░░░░░░░   24.43 % 
🌆 Daytime                2757 commits        ███████████░░░░░░░░░░░░░░   43.37 % 
🌃 Evening                1806 commits        ███████░░░░░░░░░░░░░░░░░░   28.41 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   937 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Tuesday                  881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.86 % 
Wednesday                790 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.43 % 
Thursday                 842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.81 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.85 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 39 mins       ███████████████░░░░░░░░░░   61.05 % 
YAML                     3 hrs 4 mins        █████░░░░░░░░░░░░░░░░░░░░   21.73 % 
Markdown                 1 hr 37 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.45 % 
SSH Config               18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.22 % 
Diff                     12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.42 % 

🔥 Editors: 
Zsh                      8 hrs 39 mins       ███████████████░░░░░░░░░░   61.05 % 
VS Code                  4 hrs 9 mins        ███████░░░░░░░░░░░░░░░░░░   29.31 % 
Obsidian                 1 hr 16 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.04 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.60 % 

💻 Operating System: 
Linux                    14 hrs 11 mins      █████████████████████████   100.00 % 
```


 Last Updated on 08/07/2024 00:40:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
