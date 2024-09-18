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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C767%20hrs%2058%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1689 commits        ██████░░░░░░░░░░░░░░░░░░░   25.24 % 
🌆 Daytime                2869 commits        ███████████░░░░░░░░░░░░░░   42.87 % 
🌃 Evening                1886 commits        ███████░░░░░░░░░░░░░░░░░░   28.18 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.71 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1000 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.94 % 
Tuesday                  961 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.36 % 
Wednesday                858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Thursday                 895 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Friday                   870 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Saturday                 1046 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.63 % 
Sunday                   1062 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.87 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 10 mins      ██████████████░░░░░░░░░░░   55.21 % 
YAML                     6 hrs 16 mins       █████████░░░░░░░░░░░░░░░░   34.08 % 
Markdown                 52 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.73 % 
Terraform                26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.41 % 
Other                    21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.99 % 

🔥 Editors: 
Zsh                      10 hrs 10 mins      ██████████████░░░░░░░░░░░   55.21 % 
VS Code                  7 hrs 14 mins       ██████████░░░░░░░░░░░░░░░   39.29 % 
Obsidian                 42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 
Vim                      17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.62 % 

💻 Operating System: 
Linux                    18 hrs 24 mins      █████████████████████████   100.00 % 
```


 Last Updated on 18/09/2024 00:47:38 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
