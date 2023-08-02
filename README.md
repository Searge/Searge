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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C170%20hrs%206%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1204 commits        ██████░░░░░░░░░░░░░░░░░░░   22.58 % 
🌆 Daytime                2405 commits        ███████████░░░░░░░░░░░░░░   45.11 % 
🌃 Evening                1513 commits        ███████░░░░░░░░░░░░░░░░░░   28.38 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.92 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   770 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.44 % 
Tuesday                  716 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.43 % 
Wednesday                684 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.83 % 
Thursday                 754 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   769 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.43 % 
Saturday                 829 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.55 % 
Sunday                   809 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.18 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 43 mins       ███████████░░░░░░░░░░░░░░   45.96 % 
Markdown                 3 hrs 39 mins       ███████░░░░░░░░░░░░░░░░░░   29.33 % 
Bash                     2 hrs 53 mins       ██████░░░░░░░░░░░░░░░░░░░   23.14 % 
Git Config               5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.71 % 
Nginx                    2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.36 % 

🔥 Editors: 
VS Code                  9 hrs 13 mins       ██████████████████░░░░░░░   74.00 % 
Obsidian                 3 hrs 14 mins       ██████░░░░░░░░░░░░░░░░░░░   25.94 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.07 % 

💻 Operating System: 
Linux                    12 hrs 28 mins      █████████████████████████   100.00 % 
```


 Last Updated on 02/08/2023 00:09:12 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
