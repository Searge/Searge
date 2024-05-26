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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C526%20hrs%209%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1494 commits        ██████░░░░░░░░░░░░░░░░░░░   24.19 % 
🌆 Daytime                2686 commits        ███████████░░░░░░░░░░░░░░   43.48 % 
🌃 Evening                1757 commits        ███████░░░░░░░░░░░░░░░░░░   28.44 % 
🌙 Night                  240 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.89 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   892 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.44 % 
Tuesday                  834 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.50 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.95 % 
Thursday                 826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Friday                   833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.49 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.87 % 
Sunday                   1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.38 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 14 mins      ████████████████░░░░░░░░░   62.28 % 
YAML                     5 hrs 17 mins       ███████░░░░░░░░░░░░░░░░░░   26.97 % 
Markdown                 1 hr 2 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.35 % 
Nix                      29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.52 % 
Other                    17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.46 % 

🔥 Editors: 
Zsh                      12 hrs 14 mins      ████████████████░░░░░░░░░   62.28 % 
VS Code                  6 hrs 39 mins       ████████░░░░░░░░░░░░░░░░░   33.90 % 
Obsidian                 40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.47 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.35 % 

💻 Operating System: 
Linux                    19 hrs 38 mins      █████████████████████████   100.00 % 
```


 Last Updated on 26/05/2024 00:38:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
