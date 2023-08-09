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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C172%20hrs%2054%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1219 commits        ██████░░░░░░░░░░░░░░░░░░░   22.50 % 
🌆 Daytime                2446 commits        ███████████░░░░░░░░░░░░░░   45.15 % 
🌃 Evening                1543 commits        ███████░░░░░░░░░░░░░░░░░░   28.48 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.86 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.53 % 
Tuesday                  730 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.48 % 
Wednesday                690 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.74 % 
Thursday                 765 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.12 % 
Friday                   771 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.23 % 
Saturday                 838 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
Sunday                   836 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.43 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 41 mins       ████████████████████████░   94.04 % 
YAML                     9 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   04.11 % 
Bash                     3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.44 % 
PHP                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.13 % 
Other                    0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.10 % 

🔥 Editors: 
Obsidian                 3 hrs 24 mins       ██████████████████████░░░   87.05 % 
VS Code                  25 mins             ███░░░░░░░░░░░░░░░░░░░░░░   10.98 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.97 % 

💻 Operating System: 
Linux                    2 hrs 28 mins       ████████████████░░░░░░░░░   62.94 % 
Windows                  1 hr 27 mins        █████████░░░░░░░░░░░░░░░░   37.06 % 
```


 Last Updated on 09/08/2023 00:09:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
