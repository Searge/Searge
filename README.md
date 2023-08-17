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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C178%20hrs%2025%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1311 commits        ██████░░░░░░░░░░░░░░░░░░░   22.70 % 
🌆 Daytime                2604 commits        ███████████░░░░░░░░░░░░░░   45.08 % 
🌃 Evening                1640 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   814 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Tuesday                  754 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Wednesday                772 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Thursday                 817 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   809 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.01 % 
Saturday                 890 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.41 % 
Sunday                   920 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.93 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 48 mins       ███████████████░░░░░░░░░░   61.57 % 
Markdown                 2 hrs 24 mins       ██████░░░░░░░░░░░░░░░░░░░   25.51 % 
Bash                     25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.50 % 
Other                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.37 % 
conf                     8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.57 % 

🔥 Editors: 
VS Code                  6 hrs 46 mins       ██████████████████░░░░░░░   71.73 % 
Obsidian                 2 hrs 21 mins       ██████░░░░░░░░░░░░░░░░░░░   25.00 % 
Vim                      12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.28 % 
Neovim                   5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.00 % 

💻 Operating System: 
Linux                    9 hrs 17 mins       █████████████████████████   98.55 % 
Windows                  8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.45 % 
```


 Last Updated on 17/08/2023 00:08:57 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
