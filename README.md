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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C166%20hrs%2051%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1201 commits        ██████░░░░░░░░░░░░░░░░░░░   22.57 % 
🌆 Daytime                2400 commits        ███████████░░░░░░░░░░░░░░   45.10 % 
🌃 Evening                1511 commits        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   765 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.38 % 
Tuesday                  712 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Wednesday                684 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.85 % 
Thursday                 753 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.15 % 
Friday                   769 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.45 % 
Saturday                 829 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.58 % 
Sunday                   809 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.20 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 4 mins        ███████████░░░░░░░░░░░░░░   45.77 % 
Markdown                 3 hrs 36 mins       ████████░░░░░░░░░░░░░░░░░   32.64 % 
Bash                     2 hrs 8 mins        █████░░░░░░░░░░░░░░░░░░░░   19.41 % 
INI                      8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.29 % 
Git Config               5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.80 % 

🔥 Editors: 
VS Code                  8 hrs 4 mins        ██████████████████░░░░░░░   72.88 % 
Obsidian                 2 hrs 59 mins       ███████░░░░░░░░░░░░░░░░░░   27.05 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.08 % 

💻 Operating System: 
Linux                    11 hrs 4 mins       █████████████████████████   100.00 % 
```


 Last Updated on 31/07/2023 00:09:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
