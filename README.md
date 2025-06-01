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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C406%20hrs%2048%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1861 commits        ███████░░░░░░░░░░░░░░░░░░   26.03 % 
🌆 Daytime                2984 commits        ██████████░░░░░░░░░░░░░░░   41.74 % 
🌃 Evening                2047 commits        ███████░░░░░░░░░░░░░░░░░░   28.63 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.59 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 49 mins       ████████████░░░░░░░░░░░░░   48.34 % 
Python                   4 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   23.24 % 
YAML                     2 hrs 52 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.77 % 
PHP                      40 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.69 % 
Other                    30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.76 % 

🔥 Editors: 
VS Code                  9 hrs 7 mins        ████████████░░░░░░░░░░░░░   49.94 % 
Zsh                      8 hrs 49 mins       ████████████░░░░░░░░░░░░░   48.34 % 
Obsidian                 17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.56 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.16 % 

💻 Operating System: 
Linux                    18 hrs 15 mins      █████████████████████████   100.00 % 
```


 Last Updated on 01/06/2025 00:08:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
