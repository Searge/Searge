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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C185%20hrs%2055%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1323 commits        ██████░░░░░░░░░░░░░░░░░░░   22.82 % 
🌆 Daytime                2611 commits        ███████████░░░░░░░░░░░░░░   45.03 % 
🌃 Evening                1643 commits        ███████░░░░░░░░░░░░░░░░░░   28.34 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   814 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Tuesday                  754 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Wednesday                779 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.44 % 
Thursday                 819 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   809 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Saturday                 900 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.52 % 
Sunday                   923 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.92 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 38 mins       ███████████████░░░░░░░░░░   58.13 % 
Markdown                 2 hrs 44 mins       ██████░░░░░░░░░░░░░░░░░░░   24.00 % 
Bash                     47 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.94 % 
Other                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.61 % 
PHP                      14 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.13 % 

🔥 Editors: 
VS Code                  8 hrs 26 mins       ██████████████████░░░░░░░   73.88 % 
Obsidian                 2 hrs 40 mins       ██████░░░░░░░░░░░░░░░░░░░   23.41 % 
Vim                      12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.88 % 
Neovim                   5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.82 % 

💻 Operating System: 
Linux                    11 hrs 25 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/08/2023 00:09:56 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
