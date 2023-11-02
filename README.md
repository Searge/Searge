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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C301%20hrs%2053%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1469 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                2927 commits        ███████████░░░░░░░░░░░░░░   44.95 % 
🌃 Evening                1889 commits        ███████░░░░░░░░░░░░░░░░░░   29.01 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.49 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   950 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.59 % 
Tuesday                  835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Wednesday                835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Thursday                 914 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Friday                   844 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.96 % 
Saturday                 974 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.96 % 
Sunday                   1160 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.81 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     3 hrs 37 mins       ███████████░░░░░░░░░░░░░░   42.20 % 
Markdown                 2 hrs 58 mins       █████████░░░░░░░░░░░░░░░░   34.67 % 
Other                    39 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.61 % 
VCL                      21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.21 % 
Bash                     21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.13 % 

🔥 Editors: 
VS Code                  5 hrs 34 mins       ████████████████░░░░░░░░░   64.82 % 
Obsidian                 2 hrs 35 mins       ████████░░░░░░░░░░░░░░░░░   30.19 % 
Vim                      18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.50 % 
Sublime Text             7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.49 % 

💻 Operating System: 
Linux                    8 hrs 35 mins       █████████████████████████   100.00 % 
```


 Last Updated on 02/11/2023 00:09:44 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
