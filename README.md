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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C671%20hrs%2045%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1600 commits        ██████░░░░░░░░░░░░░░░░░░░   24.61 % 
🌆 Daytime                2816 commits        ███████████░░░░░░░░░░░░░░   43.32 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.32 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   972 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.95 % 
Tuesday                  913 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Wednesday                813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.51 % 
Thursday                 857 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.18 % 
Friday                   855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Saturday                 1017 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.64 % 
Sunday                   1074 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.52 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 30 mins       ████████████████░░░░░░░░░   63.91 % 
Markdown                 2 hrs 53 mins       ███████░░░░░░░░░░░░░░░░░░   28.33 % 
YAML                     25 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.22 % 
Other                    10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.71 % 
Lua                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.34 % 

🔥 Editors: 
Zsh                      6 hrs 30 mins       ████████████████░░░░░░░░░   63.91 % 
Obsidian                 2 hrs 48 mins       ███████░░░░░░░░░░░░░░░░░░   27.55 % 
VS Code                  44 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.20 % 
Vim                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.34 % 

💻 Operating System: 
Linux                    10 hrs 11 mins      █████████████████████████   100.00 % 
```


 Last Updated on 24/07/2024 00:43:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
