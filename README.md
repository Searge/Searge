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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C255%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1405 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                2800 commits        ███████████░░░░░░░░░░░░░░   44.97 % 
🌃 Evening                1795 commits        ███████░░░░░░░░░░░░░░░░░░   28.83 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.65 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   900 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.45 % 
Tuesday                  795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Thursday                 879 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.12 % 
Friday                   820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.17 % 
Saturday                 947 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.21 % 
Sunday                   1072 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 50 mins       ██████████░░░░░░░░░░░░░░░   38.66 % 
Markdown                 5 hrs 9 mins        ███████░░░░░░░░░░░░░░░░░░   29.17 % 
Docker                   2 hrs 43 mins       ████░░░░░░░░░░░░░░░░░░░░░   15.41 % 
Bash                     30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.90 % 
Ezhil                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.33 % 

🔥 Editors: 
VS Code                  14 hrs 20 mins      ████████████████████░░░░░   80.99 % 
Obsidian                 3 hrs 17 mins       █████░░░░░░░░░░░░░░░░░░░░   18.59 % 
Vim                      4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.41 % 

💻 Operating System: 
Linux                    17 hrs 41 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/10/2023 00:09:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
