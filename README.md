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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C176%20hrs%2025%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1312 commits        ██████░░░░░░░░░░░░░░░░░░░   22.67 % 
🌆 Daytime                2602 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                1650 commits        ███████░░░░░░░░░░░░░░░░░░   28.51 % 
🌙 Night                  223 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   816 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.10 % 
Tuesday                  764 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.20 % 
Wednesday                779 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.46 % 
Thursday                 821 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Friday                   815 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Saturday                 887 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.33 % 
Sunday                   905 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     2 hrs 10 mins       █████████████░░░░░░░░░░░░   53.03 % 
Markdown                 1 hr 12 mins        ███████░░░░░░░░░░░░░░░░░░   29.35 % 
Bash                     25 mins             ███░░░░░░░░░░░░░░░░░░░░░░   10.17 % 
Other                    7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.07 % 
Docker                   5 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.07 % 

🔥 Editors: 
VS Code                  2 hrs 46 mins       █████████████████░░░░░░░░   67.69 % 
Obsidian                 1 hr 10 mins        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
Neovim                   5 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.29 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.62 % 

💻 Operating System: 
Linux                    3 hrs 49 mins       ███████████████████████░░   92.99 % 
Windows                  17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.01 % 
```


 Last Updated on 16/08/2023 00:09:09 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
