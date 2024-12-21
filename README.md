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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C024%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1695 commits        ██████░░░░░░░░░░░░░░░░░░░   25.26 % 
🌆 Daytime                2847 commits        ███████████░░░░░░░░░░░░░░   42.43 % 
🌃 Evening                1914 commits        ███████░░░░░░░░░░░░░░░░░░   28.52 % 
🌙 Night                  254 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1007 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.01 % 
Tuesday                  931 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.87 % 
Wednesday                898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Thursday                 899 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   883 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Saturday                 1060 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.80 % 
Sunday                   1032 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.38 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 48 mins       ███████████░░░░░░░░░░░░░░   45.67 % 
Markdown                 3 hrs 58 mins       ██████░░░░░░░░░░░░░░░░░░░   23.19 % 
Go                       1 hr 48 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.58 % 
YAML                     1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.12 % 
Emacs Lisp               32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.19 % 

🔥 Editors: 
Zsh                      7 hrs 48 mins       ███████████░░░░░░░░░░░░░░   45.67 % 
VS Code                  7 hrs 42 mins       ███████████░░░░░░░░░░░░░░   45.02 % 
Obsidian                 1 hr 27 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.50 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.64 % 
Cursor                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.16 % 

💻 Operating System: 
Linux                    17 hrs 6 mins       █████████████████████████   100.00 % 
```


 Last Updated on 21/12/2024 00:57:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
