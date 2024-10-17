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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C844%20hrs%2018%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1652 commits        ██████░░░░░░░░░░░░░░░░░░░   25.26 % 
🌆 Daytime                2796 commits        ███████████░░░░░░░░░░░░░░   42.75 % 
🌃 Evening                1844 commits        ███████░░░░░░░░░░░░░░░░░░   28.20 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   944 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.43 % 
Tuesday                  896 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.70 % 
Wednesday                862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.18 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.36 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.36 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 48 mins       ████████████░░░░░░░░░░░░░   46.06 % 
sh                       6 hrs 53 mins       ██████████░░░░░░░░░░░░░░░   40.66 % 
Markdown                 55 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.45 % 
DNS Zone                 47 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.65 % 
Other                    21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.11 % 

🔥 Editors: 
VS Code                  8 hrs 55 mins       █████████████░░░░░░░░░░░░   52.69 % 
Zsh                      6 hrs 53 mins       ██████████░░░░░░░░░░░░░░░   40.66 % 
Obsidian                 54 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.39 % 
Vim                      12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.27 % 

💻 Operating System: 
Linux                    16 hrs 56 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/10/2024 00:48:59 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
