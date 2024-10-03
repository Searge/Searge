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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C804%20hrs%2036%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1950 commits        ██████░░░░░░░░░░░░░░░░░░░   25.83 % 
🌆 Daytime                3000 commits        ██████████░░░░░░░░░░░░░░░   39.74 % 
🌃 Evening                2301 commits        ████████░░░░░░░░░░░░░░░░░   30.48 % 
🌙 Night                  298 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.95 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1053 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Tuesday                  981 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Wednesday                923 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.23 % 
Thursday                 942 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.48 % 
Friday                   895 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.86 % 
Saturday                 1414 commits        █████░░░░░░░░░░░░░░░░░░░░   18.73 % 
Sunday                   1341 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.76 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 45 mins       █████████████░░░░░░░░░░░░   52.77 % 
YAML                     6 hrs 23 mins       █████████░░░░░░░░░░░░░░░░   34.52 % 
Markdown                 1 hr 57 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.59 % 
Bash                     16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.52 % 
Other                    6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.56 % 

🔥 Editors: 
Zsh                      9 hrs 45 mins       █████████████░░░░░░░░░░░░   52.77 % 
VS Code                  7 hrs 15 mins       ██████████░░░░░░░░░░░░░░░   39.24 % 
Obsidian                 1 hr 18 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.10 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.89 % 

💻 Operating System: 
Linux                    18 hrs 29 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/10/2024 00:49:07 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
