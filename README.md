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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C604%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1531 commits        ██████░░░░░░░░░░░░░░░░░░░   24.23 % 
🌆 Daytime                2719 commits        ███████████░░░░░░░░░░░░░░   43.04 % 
🌃 Evening                1825 commits        ███████░░░░░░░░░░░░░░░░░░   28.89 % 
🌙 Night                  243 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   918 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.53 % 
Tuesday                  858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.58 % 
Wednesday                795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.58 % 
Thursday                 831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Friday                   827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.09 % 
Saturday                 1037 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.41 % 
Sunday                   1052 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.65 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 57 mins       ███████████████████░░░░░░   76.38 % 
YAML                     2 hrs 5 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.81 % 
JSON                     27 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
Other                    8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.15 % 
Markdown                 2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.37 % 

🔥 Editors: 
Zsh                      8 hrs 57 mins       ███████████████████░░░░░░   76.38 % 
VS Code                  2 hrs 43 mins       ██████░░░░░░░░░░░░░░░░░░░   23.21 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.40 % 

💻 Operating System: 
Linux                    11 hrs 44 mins      █████████████████████████   100.00 % 
```


 Last Updated on 23/06/2024 00:40:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
