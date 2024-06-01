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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C552%20hrs%2042%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1506 commits        ██████░░░░░░░░░░░░░░░░░░░   24.26 % 
🌆 Daytime                2701 commits        ███████████░░░░░░░░░░░░░░   43.50 % 
🌃 Evening                1762 commits        ███████░░░░░░░░░░░░░░░░░░   28.38 % 
🌙 Night                  240 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   899 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.48 % 
Tuesday                  849 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.67 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Friday                   834 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.43 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.78 % 
Sunday                   1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.41 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     12 hrs 44 mins      ██████████░░░░░░░░░░░░░░░   41.92 % 
sh                       12 hrs 18 mins      ██████████░░░░░░░░░░░░░░░   40.47 % 
Markdown                 2 hrs 42 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.88 % 
Bash                     1 hr 28 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   04.85 % 
Other                    28 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.55 % 

🔥 Editors: 
VS Code                  15 hrs 23 mins      █████████████░░░░░░░░░░░░   50.63 % 
Zsh                      12 hrs 18 mins      ██████████░░░░░░░░░░░░░░░   40.47 % 
Obsidian                 2 hrs 26 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.02 % 
Vim                      16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.88 % 

💻 Operating System: 
Linux                    30 hrs 18 mins      █████████████████████████   99.65 % 
Windows                  6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.35 % 
```


 Last Updated on 01/06/2024 00:42:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
