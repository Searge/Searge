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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C423%20hrs%2054%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1531 commits        ██████░░░░░░░░░░░░░░░░░░░   22.84 % 
🌆 Daytime                2982 commits        ███████████░░░░░░░░░░░░░░   44.49 % 
🌃 Evening                1957 commits        ███████░░░░░░░░░░░░░░░░░░   29.20 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.48 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   942 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.05 % 
Tuesday                  839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.52 % 
Wednesday                889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Thursday                 939 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.01 % 
Friday                   860 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.83 % 
Saturday                 1006 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.01 % 
Sunday                   1228 commits        █████░░░░░░░░░░░░░░░░░░░░   18.32 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr                ████████░░░░░░░░░░░░░░░░░   32.20 % 
Markdown                 41 mins             █████░░░░░░░░░░░░░░░░░░░░   21.99 % 
Other                    41 mins             █████░░░░░░░░░░░░░░░░░░░░   21.93 % 
INI                      22 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.13 % 
Docker                   17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.15 % 

🔥 Editors: 
VS Code                  2 hrs 22 mins       ███████████████████░░░░░░   75.96 % 
Obsidian                 37 mins             █████░░░░░░░░░░░░░░░░░░░░   20.11 % 
Vim                      7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 

💻 Operating System: 
Linux                    3 hrs 7 mins        █████████████████████████   100.00 % 
```


 Last Updated on 28/02/2024 00:08:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
