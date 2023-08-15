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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C174%20hrs%2051%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1312 commits        ██████░░░░░░░░░░░░░░░░░░░   22.67 % 
🌆 Daytime                2602 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                1650 commits        ███████░░░░░░░░░░░░░░░░░░   28.51 % 
🌙 Night                  223 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   816 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.10 % 
Tuesday                  764 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.20 % 
Wednesday                779 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.46 % 
Thursday                 821 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Friday                   815 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Saturday                 887 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.33 % 
Sunday                   905 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 16 mins       ████████████████░░░░░░░░░   64.44 % 
YAML                     1 hr 4 mins         ████████░░░░░░░░░░░░░░░░░   30.47 % 
Bash                     7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.58 % 
desktop                  2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.28 % 
Git                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.23 % 

🔥 Editors: 
Obsidian                 2 hrs 1 min         ██████████████░░░░░░░░░░░   57.58 % 
VS Code                  1 hr 26 mins        ██████████░░░░░░░░░░░░░░░   40.91 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

💻 Operating System: 
Linux                    1 hr 49 mins        █████████████░░░░░░░░░░░░   51.90 % 
Windows                  1 hr 41 mins        ████████████░░░░░░░░░░░░░   48.10 % 
```


 Last Updated on 15/08/2023 00:08:59 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
