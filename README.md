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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C666%20hrs-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1585 commits        ██████░░░░░░░░░░░░░░░░░░░   24.62 % 
🌆 Daytime                2786 commits        ███████████░░░░░░░░░░░░░░   43.27 % 
🌃 Evening                1824 commits        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   958 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.88 % 
Tuesday                  898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Wednesday                809 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.56 % 
Thursday                 853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.69 % 
Sunday                   1072 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.65 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 23 mins       ██████████████████░░░░░░░   72.55 % 
YAML                     1 hr 24 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.81 % 
Markdown                 1 hr 11 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.24 % 
Text                     16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.18 % 
Lua                      15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.96 % 

🔥 Editors: 
Zsh                      9 hrs 23 mins       ██████████████████░░░░░░░   72.55 % 
VS Code                  2 hrs 1 min         ████░░░░░░░░░░░░░░░░░░░░░   15.61 % 
Obsidian                 1 hr 11 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.24 % 
Vim                      20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.60 % 

💻 Operating System: 
Linux                    12 hrs 56 mins      █████████████████████████   100.00 % 
```


 Last Updated on 19/07/2024 03:54:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
