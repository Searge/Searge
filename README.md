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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C472%20hrs%2020%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   24.33 % 
🌆 Daytime                2725 commits        ███████████░░░░░░░░░░░░░░   43.02 % 
🌃 Evening                1815 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  253 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   903 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.26 % 
Tuesday                  816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
Wednesday                839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.48 % 
Saturday                 1022 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.14 % 
Sunday                   1060 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.74 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     7 hrs 59 mins       ██████████████░░░░░░░░░░░   57.77 % 
Markdown                 2 hrs 33 mins       █████░░░░░░░░░░░░░░░░░░░░   18.52 % 
sh                       1 hr 32 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.09 % 
Bash                     28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.45 % 
Other                    23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.84 % 

🔥 Editors: 
VS Code                  9 hrs 16 mins       █████████████████░░░░░░░░   67.08 % 
Zsh                      1 hr 32 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.09 % 
Obsidian                 1 hr 28 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.67 % 
Vim                      1 hr 21 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.82 % 
Sublime Text             11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.33 % 

💻 Operating System: 
Linux                    13 hrs 49 mins      █████████████████████████   100.00 % 
```


 Last Updated on 08/05/2024 00:36:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
