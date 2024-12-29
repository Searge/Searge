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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C040%20hrs%2050%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1711 commits        ██████░░░░░░░░░░░░░░░░░░░   25.36 % 
🌆 Daytime                2854 commits        ███████████░░░░░░░░░░░░░░   42.30 % 
🌃 Evening                1924 commits        ███████░░░░░░░░░░░░░░░░░░   28.52 % 
🌙 Night                  258 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 32 mins       ███████████████░░░░░░░░░░   58.81 % 
Markdown                 1 hr 25 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.80 % 
Go                       1 hr 21 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.37 % 
JSON                     54 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.57 % 
YAML                     51 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.29 % 

🔥 Editors: 
Zsh                      9 hrs 32 mins       ███████████████░░░░░░░░░░   58.81 % 
VS Code                  5 hrs 8 mins        ████████░░░░░░░░░░░░░░░░░   31.71 % 
Obsidian                 1 hr 18 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.11 % 
Vim                      13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.37 % 

💻 Operating System: 
Linux                    16 hrs 12 mins      █████████████████████████   100.00 % 
```


 Last Updated on 29/12/2024 00:47:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
