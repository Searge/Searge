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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C154%20hrs%2046%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1211 commits        ██████░░░░░░░░░░░░░░░░░░░   22.40 % 
🌆 Daytime                2435 commits        ███████████░░░░░░░░░░░░░░   45.04 % 
🌃 Evening                1550 commits        ███████░░░░░░░░░░░░░░░░░░   28.67 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   776 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.35 % 
Tuesday                  723 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Wednesday                697 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Thursday                 767 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Friday                   777 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.37 % 
Saturday                 843 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.59 % 
Sunday                   823 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 29 mins       ████████████░░░░░░░░░░░░░   49.78 % 
YAML                     2 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   24.76 % 
Bash                     43 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.04 % 
Other                    42 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.79 % 
INI                      19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.63 % 

🔥 Editors: 
VS Code                  4 hrs 59 mins       ██████████████░░░░░░░░░░░   55.24 % 
Obsidian                 3 hrs 57 mins       ███████████░░░░░░░░░░░░░░   43.72 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.04 % 

💻 Operating System: 
Linux                    9 hrs 2 mins        █████████████████████████   100.00 % 
```


 Last Updated on 24/07/2023 00:09:36 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
