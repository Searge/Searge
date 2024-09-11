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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C752%20hrs%206%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1945 commits        ██████░░░░░░░░░░░░░░░░░░░   25.58 % 
🌆 Daytime                3021 commits        ██████████░░░░░░░░░░░░░░░   39.73 % 
🌃 Evening                2346 commits        ████████░░░░░░░░░░░░░░░░░   30.86 % 
🌙 Night                  291 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1070 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  974 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
Wednesday                913 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.01 % 
Thursday                 943 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.40 % 
Friday                   879 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.56 % 
Saturday                 1448 commits        █████░░░░░░░░░░░░░░░░░░░░   19.05 % 
Sunday                   1376 commits        █████░░░░░░░░░░░░░░░░░░░░   18.10 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       4 hrs 20 mins       ███████████████░░░░░░░░░░   58.14 % 
YAML                     2 hrs 2 mins        ███████░░░░░░░░░░░░░░░░░░   27.48 % 
Markdown                 45 mins             ███░░░░░░░░░░░░░░░░░░░░░░   10.08 % 
Bash                     13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.11 % 
Other                    2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.53 % 

🔥 Editors: 
Zsh                      4 hrs 20 mins       ███████████████░░░░░░░░░░   58.14 % 
VS Code                  2 hrs 22 mins       ████████░░░░░░░░░░░░░░░░░   31.88 % 
Obsidian                 44 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.89 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.08 % 

💻 Operating System: 
Linux                    7 hrs 27 mins       █████████████████████████   100.00 % 
```


 Last Updated on 11/09/2024 00:47:06 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
