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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C139%20hrs%2027%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1222 commits        ██████░░░░░░░░░░░░░░░░░░░   22.29 % 
🌆 Daytime                2465 commits        ███████████░░░░░░░░░░░░░░   44.97 % 
🌃 Evening                1585 commits        ███████░░░░░░░░░░░░░░░░░░   28.91 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.36 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.30 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.25 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Saturday                 849 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.49 % 
Sunday                   833 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.20 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 8 hrs 7 mins        ████████░░░░░░░░░░░░░░░░░   33.64 % 
YAML                     7 hrs 31 mins       ████████░░░░░░░░░░░░░░░░░   31.15 % 
Bash                     3 hrs 59 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.56 % 
Terraform                57 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.96 % 
Other                    53 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.71 % 

🔥 Editors: 
VS Code                  16 hrs 53 mins      █████████████████░░░░░░░░   69.92 % 
Obsidian                 7 hrs 14 mins       ███████░░░░░░░░░░░░░░░░░░   29.98 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.10 % 

💻 Operating System: 
Linux                    24 hrs 9 mins       █████████████████████████   100.00 % 
```


 Last Updated on 11/07/2023 00:10:51 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
