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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C714%20hrs%2050%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1594 commits        ██████░░░░░░░░░░░░░░░░░░░   24.47 % 
🌆 Daytime                2830 commits        ███████████░░░░░░░░░░░░░░   43.44 % 
🌃 Evening                1850 commits        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.70 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   989 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.18 % 
Tuesday                  918 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Wednesday                807 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.39 % 
Thursday                 864 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Saturday                 1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.53 % 
Sunday                   1075 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.50 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs              █████████████░░░░░░░░░░░░   50.79 % 
YAML                     7 hrs 37 mins       █████████░░░░░░░░░░░░░░░░   35.21 % 
Markdown                 1 hr 20 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.19 % 
Bash                     58 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.48 % 
Docker                   19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.52 % 

🔥 Editors: 
Zsh                      11 hrs              █████████████░░░░░░░░░░░░   50.79 % 
VS Code                  9 hrs 11 mins       ███████████░░░░░░░░░░░░░░   42.46 % 
Obsidian                 1 hr 14 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.73 % 
Vim                      13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.02 % 

💻 Operating System: 
Linux                    21 hrs 39 mins      █████████████████████████   100.00 % 
```


 Last Updated on 13/08/2024 00:44:46 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
