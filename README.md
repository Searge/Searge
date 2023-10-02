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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C242%20hrs%2018%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1366 commits        ██████░░░░░░░░░░░░░░░░░░░   22.54 % 
🌆 Daytime                2733 commits        ███████████░░░░░░░░░░░░░░   45.11 % 
🌃 Evening                1739 commits        ███████░░░░░░░░░░░░░░░░░░   28.70 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.65 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   857 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Tuesday                  783 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.92 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.20 % 
Thursday                 856 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.47 % 
Saturday                 929 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.33 % 
Sunday                   1018 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.80 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     3 hrs 56 mins       █████████░░░░░░░░░░░░░░░░   35.21 % 
Docker                   3 hrs               ███████░░░░░░░░░░░░░░░░░░   26.88 % 
Markdown                 1 hr 42 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.22 % 
Bash                     1 hr 29 mins        ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Other                    22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.34 % 

🔥 Editors: 
VS Code                  9 hrs 57 mins       ██████████████████████░░░   88.94 % 
Obsidian                 1 hr 5 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   09.68 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.38 % 

💻 Operating System: 
Linux                    11 hrs 12 mins      █████████████████████████   100.00 % 
```


 Last Updated on 02/10/2023 00:10:28 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
