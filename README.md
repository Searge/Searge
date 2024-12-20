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
**I'm an Early 🐤** 

```text
🌞 Morning                1690 commits        ██████░░░░░░░░░░░░░░░░░░░   25.23 % 
🌆 Daytime                2842 commits        ███████████░░░░░░░░░░░░░░   42.43 % 
🌃 Evening                1912 commits        ███████░░░░░░░░░░░░░░░░░░   28.55 % 
🌙 Night                  254 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1003 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.97 % 
Tuesday                  927 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.84 % 
Wednesday                898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Thursday                 898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Friday                   880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.14 % 
Saturday                 1060 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.83 % 
Sunday                   1032 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.41 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 43 mins       ████████████░░░░░░░░░░░░░   46.64 % 
Markdown                 4 hrs               ██████░░░░░░░░░░░░░░░░░░░   24.17 % 
Go                       1 hr 19 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.96 % 
YAML                     1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.35 % 
Emacs Lisp               32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.30 % 

🔥 Editors: 
Zsh                      7 hrs 43 mins       ████████████░░░░░░░░░░░░░   46.64 % 
VS Code                  7 hrs 4 mins        ███████████░░░░░░░░░░░░░░   42.75 % 
Obsidian                 1 hr 37 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.81 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.64 % 
Cursor                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.17 % 

💻 Operating System: 
Linux                    16 hrs 32 mins      █████████████████████████   100.00 % 
```


 Last Updated on 20/12/2024 00:55:39 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
