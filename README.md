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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C228%20hrs%2055%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1361 commits        ██████░░░░░░░░░░░░░░░░░░░   22.60 % 
🌆 Daytime                2714 commits        ███████████░░░░░░░░░░░░░░   45.08 % 
🌃 Evening                1725 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.67 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   849 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.10 % 
Tuesday                  775 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.87 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Thursday                 851 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.13 % 
Friday                   815 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.54 % 
Saturday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.40 % 
Sunday                   1004 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     8 hrs 36 mins       ████████████░░░░░░░░░░░░░   48.06 % 
Markdown                 3 hrs 35 mins       █████░░░░░░░░░░░░░░░░░░░░   20.05 % 
Bash                     1 hr 31 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.54 % 
Ezhil                    1 hr 3 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.89 % 
Jinja2                   38 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.63 % 

🔥 Editors: 
VS Code                  15 hrs              █████████████████████░░░░   83.90 % 
Obsidian                 2 hrs 39 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.88 % 
Vim                      9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.88 % 
Sublime Text             3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.34 % 

💻 Operating System: 
Linux                    17 hrs 49 mins      █████████████████████████   99.62 % 
Windows                  4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.38 % 
```


 Last Updated on 21/09/2023 00:09:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
