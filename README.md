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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C211%20hrs%2032%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1358 commits        ██████░░░░░░░░░░░░░░░░░░░   22.59 % 
🌆 Daytime                2709 commits        ███████████░░░░░░░░░░░░░░   45.07 % 
🌃 Evening                1723 commits        ███████░░░░░░░░░░░░░░░░░░   28.66 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.68 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   845 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.06 % 
Tuesday                  770 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Thursday                 850 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   815 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.56 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.42 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.70 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 5 hrs 27 mins       ██████████░░░░░░░░░░░░░░░   41.88 % 
YAML                     3 hrs 3 mins        ██████░░░░░░░░░░░░░░░░░░░   23.50 % 
INI                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.56 % 
PHP                      33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.31 % 
Bash                     32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.13 % 

🔥 Editors: 
VS Code                  8 hrs 27 mins       ████████████████░░░░░░░░░   64.94 % 
Obsidian                 4 hrs 29 mins       █████████░░░░░░░░░░░░░░░░   34.48 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.57 % 

💻 Operating System: 
Linux                    12 hrs 49 mins      █████████████████████████   98.42 % 
Windows                  12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.58 % 
```


 Last Updated on 14/09/2023 00:09:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
