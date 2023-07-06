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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C118%20hrs%2056%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1208 commits        ██████░░░░░░░░░░░░░░░░░░░   22.26 % 
🌆 Daytime                2438 commits        ███████████░░░░░░░░░░░░░░   44.93 % 
🌃 Evening                1570 commits        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   783 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.43 % 
Tuesday                  729 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.44 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.39 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.47 % 
Saturday                 845 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.57 % 
Sunday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 9 hrs 48 mins       ██████████████░░░░░░░░░░░   55.09 % 
YAML                     3 hrs 12 mins       █████░░░░░░░░░░░░░░░░░░░░   18.04 % 
Bash                     2 hrs 40 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.99 % 
Other                    1 hr 3 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.90 % 
JavaScript               32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.00 % 

🔥 Editors: 
Obsidian                 9 hrs 6 mins        █████████████░░░░░░░░░░░░   51.18 % 
VS Code                  8 hrs 36 mins       ████████████░░░░░░░░░░░░░   48.33 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.49 % 

💻 Operating System: 
Linux                    17 hrs 48 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/07/2023 00:11:17 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
