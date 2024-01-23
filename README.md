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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C401%20hrs%203%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1538 commits        ██████░░░░░░░░░░░░░░░░░░░   22.67 % 
🌆 Daytime                3037 commits        ███████████░░░░░░░░░░░░░░   44.77 % 
🌃 Evening                1970 commits        ███████░░░░░░░░░░░░░░░░░░   29.04 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.52 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1003 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
Tuesday                  899 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Wednesday                878 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.94 % 
Thursday                 942 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.89 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.59 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Sunday                   1210 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.84 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 28 mins        ████████░░░░░░░░░░░░░░░░░   33.62 % 
Lua                      1 hr 18 mins        ███████░░░░░░░░░░░░░░░░░░   29.88 % 
YAML                     34 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.22 % 
INI                      17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.53 % 
Docker                   13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.15 % 

🔥 Editors: 
VS Code                  2 hrs               ███████████░░░░░░░░░░░░░░   45.80 % 
Obsidian                 1 hr 23 mins        ████████░░░░░░░░░░░░░░░░░   31.70 % 
Vim                      59 mins             ██████░░░░░░░░░░░░░░░░░░░   22.51 % 

💻 Operating System: 
Linux                    4 hrs 22 mins       █████████████████████████   100.00 % 
```


 Last Updated on 23/01/2024 00:10:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
