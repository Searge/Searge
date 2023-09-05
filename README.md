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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C198%20hrs%2036%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1347 commits        ██████░░░░░░░░░░░░░░░░░░░   22.67 % 
🌆 Daytime                2678 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1697 commits        ███████░░░░░░░░░░░░░░░░░░   28.55 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   836 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  766 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Wednesday                793 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Thursday                 840 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.68 % 
Saturday                 918 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.45 % 
Sunday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.44 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 13 mins       █████████░░░░░░░░░░░░░░░░   37.25 % 
YAML                     2 hrs 19 mins       ███████░░░░░░░░░░░░░░░░░░   26.94 % 
Bash                     1 hr 53 mins        █████░░░░░░░░░░░░░░░░░░░░   21.81 % 
PHP                      34 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.62 % 
JSON                     20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.03 % 

🔥 Editors: 
VS Code                  5 hrs 41 mins       ████████████████░░░░░░░░░   65.83 % 
Obsidian                 2 hrs 55 mins       ████████░░░░░░░░░░░░░░░░░   33.79 % 
Zsh                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.38 % 

💻 Operating System: 
Linux                    8 hrs 39 mins       █████████████████████████   100.00 % 
```


 Last Updated on 05/09/2023 00:09:02 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
