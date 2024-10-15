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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C835%20hrs%2014%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1645 commits        ██████░░░░░░░░░░░░░░░░░░░   25.20 % 
🌆 Daytime                2794 commits        ███████████░░░░░░░░░░░░░░   42.80 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.20 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   944 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.46 % 
Tuesday                  893 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.68 % 
Wednesday                853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.53 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 35 mins       ███████████░░░░░░░░░░░░░░   45.15 % 
YAML                     8 hrs 19 mins       ███████████░░░░░░░░░░░░░░   43.73 % 
DNS Zone                 55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.82 % 
Other                    34 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.04 % 
Markdown                 21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.90 % 

🔥 Editors: 
VS Code                  9 hrs 46 mins       █████████████░░░░░░░░░░░░   51.32 % 
Zsh                      8 hrs 35 mins       ███████████░░░░░░░░░░░░░░   45.15 % 
Vim                      23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.02 % 
Obsidian                 17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

💻 Operating System: 
Linux                    19 hrs 2 mins       █████████████████████████   100.00 % 
```


 Last Updated on 15/10/2024 00:48:15 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
