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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C540%20hrs%201%20min-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1504 commits        ██████░░░░░░░░░░░░░░░░░░░   24.23 % 
🌆 Daytime                2701 commits        ███████████░░░░░░░░░░░░░░   43.52 % 
🌃 Evening                1762 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  240 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.87 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   899 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.48 % 
Tuesday                  849 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.68 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.89 % 
Thursday                 827 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.32 % 
Friday                   833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.42 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.79 % 
Sunday                   1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.42 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       12 hrs 57 mins      ████████████░░░░░░░░░░░░░   49.87 % 
YAML                     9 hrs 25 mins       █████████░░░░░░░░░░░░░░░░   36.23 % 
Markdown                 2 hrs 23 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   09.18 % 
Bash                     27 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.77 % 
Other                    20 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.33 % 

🔥 Editors: 
Zsh                      12 hrs 57 mins      ████████████░░░░░░░░░░░░░   49.87 % 
VS Code                  10 hrs 46 mins      ██████████░░░░░░░░░░░░░░░   41.42 % 
Obsidian                 2 hrs 10 mins       ██░░░░░░░░░░░░░░░░░░░░░░░   08.35 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.35 % 

💻 Operating System: 
Linux                    25 hrs 53 mins      █████████████████████████   99.60 % 
Windows                  6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.40 % 
```


 Last Updated on 29/05/2024 00:42:05 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
