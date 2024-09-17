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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C765%20hrs-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1691 commits        ██████░░░░░░░░░░░░░░░░░░░   25.21 % 
🌆 Daytime                2875 commits        ███████████░░░░░░░░░░░░░░   42.87 % 
🌃 Evening                1894 commits        ███████░░░░░░░░░░░░░░░░░░   28.24 % 
🌙 Night                  247 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.68 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.98 % 
Tuesday                  956 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.25 % 
Wednesday                862 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.85 % 
Thursday                 898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   871 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.99 % 
Saturday                 1053 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.70 % 
Sunday                   1062 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.83 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 2 mins        ██████████████░░░░░░░░░░░   56.82 % 
YAML                     4 hrs 56 mins       ████████░░░░░░░░░░░░░░░░░   31.10 % 
Markdown                 1 hr 2 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.54 % 
Terraform                26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.79 % 
Other                    21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.30 % 

🔥 Editors: 
Zsh                      9 hrs 2 mins        ██████████████░░░░░░░░░░░   56.82 % 
VS Code                  5 hrs 41 mins       █████████░░░░░░░░░░░░░░░░   35.81 % 
Obsidian                 52 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.47 % 
Vim                      18 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.89 % 

💻 Operating System: 
Linux                    15 hrs 54 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/09/2024 00:45:56 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
