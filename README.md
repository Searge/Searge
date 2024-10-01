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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C794%20hrs%2015%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1687 commits        ██████░░░░░░░░░░░░░░░░░░░   25.32 % 
🌆 Daytime                2857 commits        ███████████░░░░░░░░░░░░░░   42.88 % 
🌃 Evening                1871 commits        ███████░░░░░░░░░░░░░░░░░░   28.08 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.75 % 
Tuesday                  947 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.21 % 
Wednesday                851 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 892 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   885 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Saturday                 1034 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.52 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.07 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 29 mins       ██████████████████░░░░░░░   71.50 % 
YAML                     2 hrs 51 mins       █████░░░░░░░░░░░░░░░░░░░░   21.59 % 
Markdown                 42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.40 % 
Bash                     10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.26 % 
Other                    1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.25 % 

🔥 Editors: 
Zsh                      9 hrs 29 mins       ██████████████████░░░░░░░   71.50 % 
VS Code                  2 hrs 56 mins       ██████░░░░░░░░░░░░░░░░░░░   22.18 % 
Obsidian                 40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.07 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.26 % 

💻 Operating System: 
Linux                    13 hrs 15 mins      █████████████████████████   100.00 % 
```


 Last Updated on 01/10/2024 00:49:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
