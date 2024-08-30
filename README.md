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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C738%20hrs%2016%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1604 commits        ██████░░░░░░░░░░░░░░░░░░░   24.59 % 
🌆 Daytime                2829 commits        ███████████░░░░░░░░░░░░░░   43.37 % 
🌃 Evening                1846 commits        ███████░░░░░░░░░░░░░░░░░░   28.30 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.89 % 
Tuesday                  913 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.00 % 
Wednesday                820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   857 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.14 % 
Saturday                 1011 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.51 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       2 hrs 58 mins       █████████████░░░░░░░░░░░░   52.11 % 
Markdown                 1 hr 31 mins        ███████░░░░░░░░░░░░░░░░░░   26.75 % 
YAML                     49 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.43 % 
Bash                     12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.77 % 
Other                    4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.24 % 

🔥 Editors: 
Zsh                      2 hrs 58 mins       █████████████░░░░░░░░░░░░   52.11 % 
VS Code                  2 hrs 24 mins       ███████████░░░░░░░░░░░░░░   42.22 % 
Obsidian                 18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.45 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.22 % 

💻 Operating System: 
Linux                    5 hrs 41 mins       █████████████████████████   100.00 % 
```


 Last Updated on 30/08/2024 00:44:21 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
