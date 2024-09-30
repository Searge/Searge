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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C794%20hrs%2012%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1672 commits        ██████░░░░░░░░░░░░░░░░░░░   25.20 % 
🌆 Daytime                2851 commits        ███████████░░░░░░░░░░░░░░   42.98 % 
🌃 Evening                1863 commits        ███████░░░░░░░░░░░░░░░░░░   28.08 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   978 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Tuesday                  941 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
Wednesday                847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Thursday                 889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Saturday                 1027 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.48 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.14 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 16 mins       ███████████████████░░░░░░   77.86 % 
YAML                     1 hr 41 mins        █████░░░░░░░░░░░░░░░░░░░░   18.17 % 
Markdown                 21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.88 % 
Bash                     0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.10 % 

🔥 Editors: 
Zsh                      7 hrs 16 mins       ███████████████████░░░░░░   77.86 % 
VS Code                  1 hr 44 mins        █████░░░░░░░░░░░░░░░░░░░░   18.64 % 
Obsidian                 19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.40 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.10 % 

💻 Operating System: 
Linux                    9 hrs 20 mins       █████████████████████████   100.00 % 
```


 Last Updated on 30/09/2024 00:50:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
