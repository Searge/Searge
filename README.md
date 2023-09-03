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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C196%20hrs%2034%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1336 commits        ██████░░░░░░░░░░░░░░░░░░░   22.74 % 
🌆 Daytime                2647 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1671 commits        ███████░░░░░░░░░░░░░░░░░░   28.44 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.76 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   827 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Tuesday                  762 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.97 % 
Wednesday                786 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Thursday                 830 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   811 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.80 % 
Saturday                 909 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   950 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.17 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     3 hrs 59 mins       █████████░░░░░░░░░░░░░░░░   36.81 % 
Markdown                 2 hrs 41 mins       ██████░░░░░░░░░░░░░░░░░░░   24.71 % 
Bash                     2 hrs 1 min         █████░░░░░░░░░░░░░░░░░░░░   18.59 % 
Docker                   50 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.76 % 
PHP                      34 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.28 % 

🔥 Editors: 
VS Code                  8 hrs 34 mins       ████████████████████░░░░░   78.92 % 
Obsidian                 2 hrs 15 mins       █████░░░░░░░░░░░░░░░░░░░░   20.78 % 
Zsh                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.30 % 

💻 Operating System: 
Linux                    10 hrs 51 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/09/2023 00:10:03 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
