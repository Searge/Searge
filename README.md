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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C556%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1490 commits        ██████░░░░░░░░░░░░░░░░░░░   24.07 % 
🌆 Daytime                2687 commits        ███████████░░░░░░░░░░░░░░   43.42 % 
🌃 Evening                1775 commits        ███████░░░░░░░░░░░░░░░░░░   28.68 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   899 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.53 % 
Tuesday                  838 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.54 % 
Wednesday                787 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.72 % 
Thursday                 823 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.30 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.35 % 
Saturday                 997 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.11 % 
Sunday                   1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.46 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     11 hrs 39 mins      ███████████░░░░░░░░░░░░░░   45.79 % 
sh                       8 hrs 27 mins       ████████░░░░░░░░░░░░░░░░░   33.25 % 
Markdown                 2 hrs 49 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.13 % 
Bash                     1 hr 28 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.79 % 
Other                    19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.26 % 

🔥 Editors: 
VS Code                  14 hrs 6 mins       ██████████████░░░░░░░░░░░   55.46 % 
Zsh                      8 hrs 27 mins       ████████░░░░░░░░░░░░░░░░░   33.25 % 
Obsidian                 2 hrs 39 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.42 % 
Vim                      13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.86 % 

💻 Operating System: 
Linux                    25 hrs 20 mins      █████████████████████████   99.59 % 
Windows                  6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.41 % 
```


 Last Updated on 02/06/2024 00:40:29 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
