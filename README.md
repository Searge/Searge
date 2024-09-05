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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C746%20hrs%206%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1871 commits        ██████░░░░░░░░░░░░░░░░░░░   25.27 % 
🌆 Daytime                2972 commits        ██████████░░░░░░░░░░░░░░░   40.15 % 
🌃 Evening                2276 commits        ████████░░░░░░░░░░░░░░░░░   30.74 % 
🌙 Night                  284 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1041 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.06 % 
Tuesday                  946 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Wednesday                886 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.97 % 
Thursday                 924 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.48 % 
Friday                   868 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.72 % 
Saturday                 1391 commits        █████░░░░░░░░░░░░░░░░░░░░   18.79 % 
Sunday                   1347 commits        █████░░░░░░░░░░░░░░░░░░░░   18.20 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 1 min         ██████████████░░░░░░░░░░░   55.56 % 
YAML                     2 hrs 31 mins       ██████░░░░░░░░░░░░░░░░░░░   23.32 % 
Markdown                 1 hr 13 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.34 % 
Bash                     26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.04 % 
INI                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.69 % 

🔥 Editors: 
Zsh                      6 hrs 1 min         ██████████████░░░░░░░░░░░   55.56 % 
VS Code                  3 hrs 45 mins       █████████░░░░░░░░░░░░░░░░   34.76 % 
Obsidian                 1 hr 2 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   09.57 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.12 % 

💻 Operating System: 
Linux                    10 hrs 50 mins      █████████████████████████   100.00 % 
```


 Last Updated on 05/09/2024 00:44:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
