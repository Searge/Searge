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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C218%20hrs-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1360 commits        ██████░░░░░░░░░░░░░░░░░░░   22.59 % 
🌆 Daytime                2714 commits        ███████████░░░░░░░░░░░░░░   45.08 % 
🌃 Evening                1725 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.67 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   849 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.10 % 
Tuesday                  774 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Thursday                 851 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   815 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.54 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.40 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.68 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     4 hrs 52 mins       █████████░░░░░░░░░░░░░░░░   36.72 % 
Markdown                 4 hrs 33 mins       █████████░░░░░░░░░░░░░░░░   34.24 % 
Bash                     36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.54 % 
PHP                      33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.22 % 
Ezhil                    33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.16 % 

🔥 Editors: 
VS Code                  9 hrs 15 mins       █████████████████░░░░░░░░   69.68 % 
Obsidian                 3 hrs 55 mins       ███████░░░░░░░░░░░░░░░░░░   29.59 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.73 % 

💻 Operating System: 
Linux                    13 hrs 5 mins       █████████████████████████   98.45 % 
Windows                  12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.55 % 
```


 Last Updated on 16/09/2023 00:09:04 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
