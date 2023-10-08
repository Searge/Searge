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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C261%20hrs%2020%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1407 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                2805 commits        ███████████░░░░░░░░░░░░░░   44.98 % 
🌃 Evening                1797 commits        ███████░░░░░░░░░░░░░░░░░░   28.82 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.64 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   904 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.50 % 
Tuesday                  799 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Thursday                 880 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.11 % 
Friday                   820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Saturday                 947 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.19 % 
Sunday                   1072 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.19 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 8 hrs 52 mins       ███████████░░░░░░░░░░░░░░   42.38 % 
YAML                     6 hrs 48 mins       ████████░░░░░░░░░░░░░░░░░   32.56 % 
Docker                   2 hrs 32 mins       ███░░░░░░░░░░░░░░░░░░░░░░   12.15 % 
Bash                     40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.23 % 
Ezhil                    24 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.98 % 

🔥 Editors: 
VS Code                  13 hrs 53 mins      █████████████████░░░░░░░░   66.40 % 
Obsidian                 6 hrs 59 mins       ████████░░░░░░░░░░░░░░░░░   33.44 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.11 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.04 % 

💻 Operating System: 
Linux                    20 hrs 55 mins      █████████████████████████   100.00 % 
```


 Last Updated on 08/10/2023 00:11:00 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
