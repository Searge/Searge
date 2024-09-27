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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C789%20hrs%2024%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1671 commits        ██████░░░░░░░░░░░░░░░░░░░   25.20 % 
🌆 Daytime                2850 commits        ███████████░░░░░░░░░░░░░░   42.97 % 
🌃 Evening                1863 commits        ███████░░░░░░░░░░░░░░░░░░   28.09 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   978 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.75 % 
Tuesday                  941 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Wednesday                847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.15 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 58 mins       ███████████████░░░░░░░░░░   59.11 % 
YAML                     4 hrs 8 mins        ████████░░░░░░░░░░░░░░░░░   30.71 % 
Other                    36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.56 % 
Markdown                 24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.99 % 
DNS Zone                 12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

🔥 Editors: 
Zsh                      7 hrs 58 mins       ███████████████░░░░░░░░░░   59.11 % 
VS Code                  5 hrs 6 mins        █████████░░░░░░░░░░░░░░░░   37.95 % 
Obsidian                 21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.66 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.28 % 

💻 Operating System: 
Linux                    13 hrs 28 mins      █████████████████████████   100.00 % 
```


 Last Updated on 27/09/2024 00:51:05 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
