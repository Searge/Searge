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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C734%20hrs%2036%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1622 commits        ██████░░░░░░░░░░░░░░░░░░░   24.70 % 
🌆 Daytime                2836 commits        ███████████░░░░░░░░░░░░░░   43.19 % 
🌃 Evening                1864 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   973 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.82 % 
Tuesday                  925 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.61 % 
Thursday                 871 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Friday                   860 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Saturday                 1032 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.72 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.40 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       4 hrs 10 mins       █████████████░░░░░░░░░░░░   50.01 % 
YAML                     2 hrs 16 mins       ███████░░░░░░░░░░░░░░░░░░   27.23 % 
Bash                     29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.92 % 
Markdown                 28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.76 % 
Other                    16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.32 % 

🔥 Editors: 
Zsh                      4 hrs 8 mins        ████████████░░░░░░░░░░░░░   49.58 % 
VS Code                  3 hrs 45 mins       ███████████░░░░░░░░░░░░░░   45.08 % 
Obsidian                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.66 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.69 % 

💻 Operating System: 
Linux                    8 hrs 21 mins       █████████████████████████   100.00 % 
```


 Last Updated on 23/08/2024 00:48:47 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
