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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C414%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   22.74 % 
🌆 Daytime                3035 commits        ███████████░░░░░░░░░░░░░░   44.79 % 
🌃 Evening                1967 commits        ███████░░░░░░░░░░░░░░░░░░   29.03 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.77 % 
Tuesday                  899 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Wednesday                881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Thursday                 944 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.60 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.73 % 
Sunday                   1199 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.69 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 52 mins       ████████████████░░░░░░░░░   64.55 % 
gitrebase                42 mins             ████░░░░░░░░░░░░░░░░░░░░░   15.72 % 
Git                      14 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.52 % 
TOML                     13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.18 % 
Nix                      7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.87 % 

🔥 Editors: 
Obsidian                 1 hr 57 mins        ███████████░░░░░░░░░░░░░░   44.05 % 
VS Code                  1 hr 24 mins        ████████░░░░░░░░░░░░░░░░░   31.54 % 
Vim                      1 hr 5 mins         ██████░░░░░░░░░░░░░░░░░░░   24.42 % 

💻 Operating System: 
Linux                    4 hrs 27 mins       █████████████████████████   100.00 % 
```


 Last Updated on 06/02/2024 00:10:08 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
