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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C441%20hrs%2016%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   22.83 % 
🌆 Daytime                3010 commits        ███████████░░░░░░░░░░░░░░   44.59 % 
🌃 Evening                1966 commits        ███████░░░░░░░░░░░░░░░░░░   29.13 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.45 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   950 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.07 % 
Tuesday                  847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.55 % 
Wednesday                890 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.19 % 
Thursday                 944 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Friday                   861 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Saturday                 1023 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.16 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.30 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     2 hrs 18 mins       █████████░░░░░░░░░░░░░░░░   37.45 % 
Markdown                 1 hr 5 mins         ████░░░░░░░░░░░░░░░░░░░░░   17.72 % 
Other                    54 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Bash                     32 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.83 % 
INI                      25 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.86 % 

🔥 Editors: 
VS Code                  5 hrs 31 mins       ██████████████████████░░░   89.62 % 
Obsidian                 31 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.62 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.76 % 

💻 Operating System: 
Linux                    6 hrs 10 mins       █████████████████████████   100.00 % 
```


 Last Updated on 19/03/2024 00:09:39 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
