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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C743%20hrs%2036%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1605 commits        ██████░░░░░░░░░░░░░░░░░░░   24.60 % 
🌆 Daytime                2829 commits        ███████████░░░░░░░░░░░░░░   43.36 % 
🌃 Evening                1846 commits        ███████░░░░░░░░░░░░░░░░░░   28.30 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.88 % 
Tuesday                  913 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Wednesday                820 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Saturday                 1011 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.51 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       5 hrs 25 mins       ██████████████░░░░░░░░░░░   55.14 % 
YAML                     1 hr 52 mins        █████░░░░░░░░░░░░░░░░░░░░   19.10 % 
Markdown                 1 hr 43 mins        ████░░░░░░░░░░░░░░░░░░░░░   17.52 % 
Bash                     20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.46 % 
Other                    10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.78 % 

🔥 Editors: 
Zsh                      5 hrs 25 mins       ██████████████░░░░░░░░░░░   55.14 % 
VS Code                  3 hrs 54 mins       ██████████░░░░░░░░░░░░░░░   39.76 % 
Obsidian                 29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.97 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.13 % 

💻 Operating System: 
Linux                    9 hrs 49 mins       █████████████████████████   100.00 % 
```


 Last Updated on 01/09/2024 00:49:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
