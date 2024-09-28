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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C791%20hrs%207%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1671 commits        ██████░░░░░░░░░░░░░░░░░░░   25.19 % 
🌆 Daytime                2851 commits        ███████████░░░░░░░░░░░░░░   42.98 % 
🌃 Evening                1863 commits        ███████░░░░░░░░░░░░░░░░░░   28.09 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   978 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Tuesday                  941 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Wednesday                847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.15 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 20 mins       ██████████████░░░░░░░░░░░   56.58 % 
YAML                     5 hrs 3 mins        █████████░░░░░░░░░░░░░░░░   34.32 % 
Other                    35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.96 % 
Markdown                 24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.73 % 
DNS Zone                 12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.38 % 

🔥 Editors: 
Zsh                      8 hrs 20 mins       ██████████████░░░░░░░░░░░   56.58 % 
VS Code                  6 hrs               ██████████░░░░░░░░░░░░░░░   40.73 % 
Obsidian                 21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.43 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.26 % 

💻 Operating System: 
Linux                    14 hrs 44 mins      █████████████████████████   100.00 % 
```


 Last Updated on 28/09/2024 00:48:23 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
