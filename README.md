# Hi, I'm Searge <img src="images/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />

## An DevOps Engineer at [Smile Ukraine](https://smile-ukraine.com/en)

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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C109%20hrs%207%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1208 commits        ██████░░░░░░░░░░░░░░░░░░░   22.28 % 
🌆 Daytime                2437 commits        ███████████░░░░░░░░░░░░░░   44.94 % 
🌃 Evening                1568 commits        ███████░░░░░░░░░░░░░░░░░░   28.91 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.40 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.44 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.40 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.48 % 
Saturday                 844 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 10 hrs 36 mins      ██████████████░░░░░░░░░░░   55.61 % 
YAML                     3 hrs 45 mins       █████░░░░░░░░░░░░░░░░░░░░   19.68 % 
Other                    1 hr 38 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.58 % 
Bash                     1 hr 25 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.44 % 
VCL                      43 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 

🔥 Editors: 
VS Code                  9 hrs 53 mins       █████████████░░░░░░░░░░░░   51.88 % 
Obsidian                 8 hrs 31 mins       ███████████░░░░░░░░░░░░░░   44.69 % 
Vim                      39 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.43 % 

💻 Operating System: 
Linux                    19 hrs 3 mins       █████████████████████████   99.98 % 
Mac                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 
```


 Last Updated on 01/07/2023 00:10:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
