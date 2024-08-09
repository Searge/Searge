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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C704%20hrs%2046%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1599 commits        ██████░░░░░░░░░░░░░░░░░░░   24.52 % 
🌆 Daytime                2834 commits        ███████████░░░░░░░░░░░░░░   43.47 % 
🌃 Evening                1843 commits        ███████░░░░░░░░░░░░░░░░░░   28.27 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.98 % 
Tuesday                  922 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Wednesday                816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.52 % 
Thursday                 866 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.49 % 
Sunday                   1075 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.49 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 32 mins       █████████████████░░░░░░░░   68.05 % 
YAML                     2 hrs 51 mins       █████░░░░░░░░░░░░░░░░░░░░   20.39 % 
Markdown                 49 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.87 % 
Other                    32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.89 % 
CSS                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.83 % 

🔥 Editors: 
Zsh                      9 hrs 32 mins       █████████████████░░░░░░░░   68.05 % 
VS Code                  3 hrs 33 mins       ██████░░░░░░░░░░░░░░░░░░░   25.43 % 
Obsidian                 49 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.87 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.66 % 

💻 Operating System: 
Linux                    14 hrs              █████████████████████████   100.00 % 
```


 Last Updated on 09/08/2024 00:46:27 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
