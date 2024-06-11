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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C581%20hrs%2053%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1502 commits        ██████░░░░░░░░░░░░░░░░░░░   24.06 % 
🌆 Daytime                2714 commits        ███████████░░░░░░░░░░░░░░   43.47 % 
🌃 Evening                1788 commits        ███████░░░░░░░░░░░░░░░░░░   28.64 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   912 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.61 % 
Tuesday                  846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.55 % 
Wednesday                793 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.70 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.26 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.24 % 
Sunday                   1024 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.40 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 36 mins      █████████████░░░░░░░░░░░░   50.03 % 
YAML                     6 hrs 21 mins       ███████░░░░░░░░░░░░░░░░░░   29.95 % 
Bash                     1 hr 29 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.03 % 
Markdown                 1 hr 28 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.99 % 
Other                    24 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.96 % 

🔥 Editors: 
Zsh                      10 hrs 36 mins      █████████████░░░░░░░░░░░░   50.03 % 
VS Code                  8 hrs 33 mins       ██████████░░░░░░░░░░░░░░░   40.39 % 
Obsidian                 1 hr 5 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.11 % 
Vim                      56 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.47 % 

💻 Operating System: 
Linux                    21 hrs 12 mins      █████████████████████████   100.00 % 
```


 Last Updated on 11/06/2024 00:43:02 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
