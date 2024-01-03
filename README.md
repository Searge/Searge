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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C387%20hrs%202%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1527 commits        ██████░░░░░░░░░░░░░░░░░░░   22.70 % 
🌆 Daytime                3021 commits        ███████████░░░░░░░░░░░░░░   44.92 % 
🌃 Evening                1947 commits        ███████░░░░░░░░░░░░░░░░░░   28.95 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.43 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   995 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.79 % 
Tuesday                  888 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.20 % 
Wednesday                858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Thursday                 935 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.90 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.67 % 
Saturday                 990 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Sunday                   1208 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.96 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 20 mins       █████████████████░░░░░░░░   69.21 % 
YAML                     1 hr 45 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.51 % 
PHP                      41 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.46 % 
Other                    19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.06 % 
Bash                     12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.92 % 

🔥 Editors: 
Obsidian                 5 hrs 44 mins       ██████████████░░░░░░░░░░░   54.18 % 
VS Code                  4 hrs 41 mins       ███████████░░░░░░░░░░░░░░   44.31 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

💻 Operating System: 
Linux                    8 hrs 46 mins       █████████████████████░░░░   82.75 % 
Windows                  1 hr 49 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.25 % 
```


 Last Updated on 03/01/2024 00:09:54 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
