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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C706%20hrs%2016%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1621 commits        ██████░░░░░░░░░░░░░░░░░░░   24.68 % 
🌆 Daytime                2850 commits        ███████████░░░░░░░░░░░░░░   43.39 % 
🌃 Evening                1850 commits        ███████░░░░░░░░░░░░░░░░░░   28.17 % 
🌙 Night                  247 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.76 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.88 % 
Tuesday                  934 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.22 % 
Wednesday                829 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.62 % 
Thursday                 872 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Friday                   865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.17 % 
Saturday                 1015 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.45 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.38 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 41 mins       ███████████████░░░░░░░░░░   58.54 % 
YAML                     3 hrs 35 mins       ███████░░░░░░░░░░░░░░░░░░   27.33 % 
Markdown                 1 hr 3 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.11 % 
Other                    33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.22 % 
CSS                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.88 % 

🔥 Editors: 
Zsh                      7 hrs 41 mins       ███████████████░░░░░░░░░░   58.54 % 
VS Code                  4 hrs 12 mins       ████████░░░░░░░░░░░░░░░░░   32.08 % 
Obsidian                 1 hr 3 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.11 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.27 % 

💻 Operating System: 
Linux                    13 hrs 7 mins       █████████████████████████   100.00 % 
```


 Last Updated on 10/08/2024 00:42:29 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
