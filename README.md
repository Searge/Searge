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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C669%20hrs%204%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1585 commits        ██████░░░░░░░░░░░░░░░░░░░   24.56 % 
🌆 Daytime                2797 commits        ███████████░░░░░░░░░░░░░░   43.34 % 
🌃 Evening                1828 commits        ███████░░░░░░░░░░░░░░░░░░   28.32 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.78 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   958 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.84 % 
Tuesday                  898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.91 % 
Wednesday                809 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.53 % 
Thursday                 853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.22 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.65 % 
Sunday                   1072 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.61 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 44 mins       ███████████████░░░░░░░░░░   59.61 % 
Markdown                 2 hrs 49 mins       ██████░░░░░░░░░░░░░░░░░░░   24.95 % 
YAML                     55 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.13 % 
Text                     16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.39 % 
Other                    14 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.19 % 

🔥 Editors: 
Zsh                      6 hrs 44 mins       ███████████████░░░░░░░░░░   59.61 % 
Obsidian                 2 hrs 49 mins       ██████░░░░░░░░░░░░░░░░░░░   24.95 % 
VS Code                  1 hr 36 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.23 % 
Vim                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.21 % 

💻 Operating System: 
Linux                    11 hrs 18 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/07/2024 00:42:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
