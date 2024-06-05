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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C562%20hrs%2052%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1494 commits        ██████░░░░░░░░░░░░░░░░░░░   24.08 % 
🌆 Daytime                2694 commits        ███████████░░░░░░░░░░░░░░   43.42 % 
🌃 Evening                1779 commits        ███████░░░░░░░░░░░░░░░░░░   28.68 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   903 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.56 % 
Tuesday                  842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.57 % 
Wednesday                787 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.69 % 
Thursday                 823 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Saturday                 1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.13 % 
Sunday                   1022 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 49 mins       ████████████░░░░░░░░░░░░░   47.27 % 
YAML                     7 hrs 43 mins       █████████░░░░░░░░░░░░░░░░   37.20 % 
Markdown                 1 hr 5 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.24 % 
Bash                     1 hr 2 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   04.99 % 
Other                    25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.07 % 

🔥 Editors: 
Zsh                      9 hrs 49 mins       ████████████░░░░░░░░░░░░░   47.27 % 
VS Code                  9 hrs 34 mins       ████████████░░░░░░░░░░░░░   46.08 % 
Obsidian                 59 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.78 % 
Vim                      23 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.85 % 
Unknown Editor           0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.02 % 

💻 Operating System: 
Linux                    20 hrs 46 mins      █████████████████████████   100.00 % 
```


 Last Updated on 05/06/2024 00:39:03 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
