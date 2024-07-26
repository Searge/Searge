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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C677%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1574 commits        ██████░░░░░░░░░░░░░░░░░░░   24.42 % 
🌆 Daytime                2800 commits        ███████████░░░░░░░░░░░░░░   43.44 % 
🌃 Evening                1830 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   970 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.05 % 
Tuesday                  898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.41 % 
Thursday                 853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Friday                   846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.13 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.59 % 
Sunday                   1073 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.65 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 9 mins        ████████████░░░░░░░░░░░░░   47.25 % 
YAML                     3 hrs 49 mins       ██████░░░░░░░░░░░░░░░░░░░   25.28 % 
Markdown                 3 hrs 15 mins       █████░░░░░░░░░░░░░░░░░░░░   21.50 % 
Bash                     18 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   02.00 % 
Other                    13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.49 % 

🔥 Editors: 
Zsh                      7 hrs 9 mins        ████████████░░░░░░░░░░░░░   47.25 % 
VS Code                  4 hrs 49 mins       ████████░░░░░░░░░░░░░░░░░   31.83 % 
Obsidian                 3 hrs 10 mins       █████░░░░░░░░░░░░░░░░░░░░   20.93 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

💻 Operating System: 
Linux                    15 hrs 8 mins       █████████████████████████   100.00 % 
```


 Last Updated on 26/07/2024 00:42:43 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
