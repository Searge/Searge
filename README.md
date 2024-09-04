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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C744%20hrs%2029%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1868 commits        ██████░░░░░░░░░░░░░░░░░░░   25.25 % 
🌆 Daytime                2969 commits        ██████████░░░░░░░░░░░░░░░   40.14 % 
🌃 Evening                2276 commits        ████████░░░░░░░░░░░░░░░░░   30.77 % 
🌙 Night                  284 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1041 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  946 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.79 % 
Wednesday                880 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.90 % 
Thursday                 924 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.49 % 
Friday                   868 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.73 % 
Saturday                 1391 commits        █████░░░░░░░░░░░░░░░░░░░░   18.80 % 
Sunday                   1347 commits        █████░░░░░░░░░░░░░░░░░░░░   18.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       5 hrs 27 mins       ██████████████░░░░░░░░░░░   57.74 % 
YAML                     2 hrs 8 mins        ██████░░░░░░░░░░░░░░░░░░░   22.68 % 
Markdown                 44 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.80 % 
Bash                     27 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.91 % 
INI                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.93 % 

🔥 Editors: 
Zsh                      5 hrs 27 mins       ██████████████░░░░░░░░░░░   57.74 % 
VS Code                  3 hrs 26 mins       █████████░░░░░░░░░░░░░░░░   36.35 % 
Obsidian                 32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.78 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.13 % 

💻 Operating System: 
Linux                    9 hrs 27 mins       █████████████████████████   100.00 % 
```


 Last Updated on 04/09/2024 00:46:10 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
