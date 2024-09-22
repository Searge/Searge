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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C779%20hrs%2024%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1656 commits        ██████░░░░░░░░░░░░░░░░░░░   25.15 % 
🌆 Daytime                2827 commits        ███████████░░░░░░░░░░░░░░   42.94 % 
🌃 Evening                1853 commits        ███████░░░░░░░░░░░░░░░░░░   28.14 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.77 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   965 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.66 % 
Tuesday                  926 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.06 % 
Wednesday                846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.85 % 
Thursday                 882 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.32 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.58 % 
Sunday                   1062 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.13 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 6 mins        ████████████░░░░░░░░░░░░░   48.39 % 
YAML                     7 hrs 17 mins       ███████████░░░░░░░░░░░░░░   43.46 % 
Other                    46 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.63 % 
DNS Zone                 9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.97 % 
Markdown                 7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.73 % 

🔥 Editors: 
VS Code                  8 hrs 36 mins       █████████████░░░░░░░░░░░░   51.33 % 
Zsh                      8 hrs 6 mins        ████████████░░░░░░░░░░░░░   48.39 % 
Obsidian                 2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.24 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.04 % 

💻 Operating System: 
Linux                    16 hrs 45 mins      █████████████████████████   100.00 % 
```


 Last Updated on 22/09/2024 00:49:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
