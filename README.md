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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C153%20hrs%2034%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1232 commits        ██████░░░░░░░░░░░░░░░░░░░   22.40 % 
🌆 Daytime                2470 commits        ███████████░░░░░░░░░░░░░░   44.92 % 
🌃 Evening                1587 commits        ███████░░░░░░░░░░░░░░░░░░   28.86 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.31 % 
Tuesday                  737 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.06 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.20 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.28 % 
Saturday                 858 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.60 % 
Sunday                   833 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.15 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 20 mins       █████████████░░░░░░░░░░░░   50.30 % 
YAML                     2 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   25.93 % 
Bash                     43 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.42 % 
Other                    42 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.16 % 
INI                      19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 

🔥 Editors: 
VS Code                  4 hrs 42 mins       ██████████████░░░░░░░░░░░   54.63 % 
Obsidian                 3 hrs 49 mins       ███████████░░░░░░░░░░░░░░   44.29 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.09 % 

💻 Operating System: 
Linux                    8 hrs 37 mins       █████████████████████████   100.00 % 
```


 Last Updated on 23/07/2023 00:09:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
