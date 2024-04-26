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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C458%20hrs%202%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1484 commits        ██████░░░░░░░░░░░░░░░░░░░   24.07 % 
🌆 Daytime                2686 commits        ███████████░░░░░░░░░░░░░░   43.57 % 
🌃 Evening                1750 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.97 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   880 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.27 % 
Tuesday                  810 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.14 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.20 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.63 % 
Friday                   842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Saturday                 978 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.86 % 
Sunday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.24 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 28 mins        █████████████░░░░░░░░░░░░   51.86 % 
YAML                     35 mins             █████░░░░░░░░░░░░░░░░░░░░   20.90 % 
Config                   20 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.04 % 
Other                    12 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.42 % 
Jinja2                   5 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.37 % 

🔥 Editors: 
VS Code                  1 hr 37 mins        ██████████████░░░░░░░░░░░   56.70 % 
Obsidian                 1 hr 12 mins        ███████████░░░░░░░░░░░░░░   42.35 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.94 % 

💻 Operating System: 
Linux                    2 hrs 51 mins       █████████████████████████   100.00 % 
```


 Last Updated on 26/04/2024 00:37:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
