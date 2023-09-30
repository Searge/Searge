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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C241%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1366 commits        ██████░░░░░░░░░░░░░░░░░░░   22.60 % 
🌆 Daytime                2724 commits        ███████████░░░░░░░░░░░░░░   45.08 % 
🌃 Evening                1732 commits        ███████░░░░░░░░░░░░░░░░░░   28.66 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.66 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   857 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
Tuesday                  783 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.96 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Thursday                 856 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.17 % 
Friday                   816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.50 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.34 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.61 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     2 hrs 12 mins       ████████░░░░░░░░░░░░░░░░░   31.44 % 
Markdown                 1 hr 24 mins        █████░░░░░░░░░░░░░░░░░░░░   20.22 % 
Docker                   1 hr 17 mins        █████░░░░░░░░░░░░░░░░░░░░   18.47 % 
Bash                     1 hr 12 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.34 % 
Other                    15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.66 % 

🔥 Editors: 
VS Code                  5 hrs 41 mins       ████████████████████░░░░░   81.36 % 
Obsidian                 1 hr 13 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.48 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.16 % 

💻 Operating System: 
Linux                    6 hrs 59 mins       █████████████████████████   100.00 % 
```


 Last Updated on 30/09/2023 00:09:27 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
