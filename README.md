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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C157%20hrs%2055%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1200 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                2400 commits        ███████████░░░░░░░░░░░░░░   45.11 % 
🌃 Evening                1511 commits        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   765 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.38 % 
Tuesday                  712 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Wednesday                684 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Thursday                 753 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.15 % 
Friday                   769 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.45 % 
Saturday                 828 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   809 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 5 hrs 14 mins       ██████████████████░░░░░░░   71.73 % 
Other                    31 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.14 % 
Bash                     26 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.03 % 
YAML                     22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.15 % 
JSON                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.48 % 

🔥 Editors: 
Obsidian                 4 hrs 8 mins        ██████████████░░░░░░░░░░░   56.72 % 
VS Code                  3 hrs 7 mins        ███████████░░░░░░░░░░░░░░   42.77 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.51 % 

💻 Operating System: 
Linux                    7 hrs 18 mins       █████████████████████████   100.00 % 
```


 Last Updated on 27/07/2023 00:09:02 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
