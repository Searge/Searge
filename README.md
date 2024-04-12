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
**I'm an Early 🐤** 

```text
🌞 Morning                1414 commits        ██████░░░░░░░░░░░░░░░░░░░   23.77 % 
🌆 Daytime                2638 commits        ███████████░░░░░░░░░░░░░░   44.34 % 
🌃 Evening                1660 commits        ███████░░░░░░░░░░░░░░░░░░   27.90 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.98 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   853 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.92 % 
Friday                   830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Saturday                 921 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.48 % 
Sunday                   920 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.46 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 39 mins       ███████████████░░░░░░░░░░   60.45 % 
Other                    34 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.06 % 
Bash                     20 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.94 % 
YAML                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.91 % 
XML                      11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.25 % 

🔥 Editors: 
VS Code                  2 hrs 36 mins       ███████████████░░░░░░░░░░   59.13 % 
Obsidian                 1 hr 41 mins        ██████████░░░░░░░░░░░░░░░   38.29 % 
Vim                      6 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.58 % 

💻 Operating System: 
Linux                    4 hrs 24 mins       █████████████████████████   100.00 % 
```


 Last Updated on 12/04/2024 00:39:10 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
