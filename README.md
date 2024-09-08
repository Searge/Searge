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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C750%20hrs%208%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1919 commits        ██████░░░░░░░░░░░░░░░░░░░   25.46 % 
🌆 Daytime                3001 commits        ██████████░░░░░░░░░░░░░░░   39.81 % 
🌃 Evening                2327 commits        ████████░░░░░░░░░░░░░░░░░   30.87 % 
🌙 Night                  291 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.86 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1048 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.90 % 
Tuesday                  961 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Wednesday                905 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.01 % 
Thursday                 937 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.43 % 
Friday                   877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.63 % 
Saturday                 1434 commits        █████░░░░░░░░░░░░░░░░░░░░   19.02 % 
Sunday                   1376 commits        █████░░░░░░░░░░░░░░░░░░░░   18.25 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       3 hrs 16 mins       ██████████████░░░░░░░░░░░   57.48 % 
YAML                     1 hr 10 mins        █████░░░░░░░░░░░░░░░░░░░░   20.49 % 
Markdown                 54 mins             ████░░░░░░░░░░░░░░░░░░░░░   15.97 % 
INI                      10 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.18 % 
Bash                     7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.17 % 

🔥 Editors: 
Zsh                      3 hrs 16 mins       ██████████████░░░░░░░░░░░   57.48 % 
VS Code                  1 hr 30 mins        ███████░░░░░░░░░░░░░░░░░░   26.56 % 
Obsidian                 54 mins             ████░░░░░░░░░░░░░░░░░░░░░   15.97 % 

💻 Operating System: 
Linux                    5 hrs 42 mins       █████████████████████████   100.00 % 
```


 Last Updated on 08/09/2024 00:49:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
