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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C736%20hrs%2039%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1604 commits        ██████░░░░░░░░░░░░░░░░░░░   24.64 % 
🌆 Daytime                2819 commits        ███████████░░░░░░░░░░░░░░   43.30 % 
🌃 Evening                1844 commits        ███████░░░░░░░░░░░░░░░░░░   28.32 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.91 % 
Tuesday                  913 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Wednesday                820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.59 % 
Thursday                 862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Friday                   857 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Saturday                 1011 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.53 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.54 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       1 hr 44 mins        ████████████░░░░░░░░░░░░░   46.87 % 
Markdown                 1 hr 21 mins        █████████░░░░░░░░░░░░░░░░   36.53 % 
YAML                     31 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.02 % 
Other                    2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.32 % 
Bash                     1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.70 % 

🔥 Editors: 
Zsh                      1 hr 44 mins        ████████████░░░░░░░░░░░░░   46.87 % 
VS Code                  1 hr 39 mins        ███████████░░░░░░░░░░░░░░   44.75 % 
Obsidian                 18 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.38 % 

💻 Operating System: 
Linux                    3 hrs 42 mins       █████████████████████████   100.00 % 
```


 Last Updated on 29/08/2024 00:42:58 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
