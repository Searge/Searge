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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C726%20hrs%2015%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1607 commits        ██████░░░░░░░░░░░░░░░░░░░   24.56 % 
🌆 Daytime                2843 commits        ███████████░░░░░░░░░░░░░░   43.44 % 
🌃 Evening                1850 commits        ███████░░░░░░░░░░░░░░░░░░   28.27 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.73 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   987 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.08 % 
Tuesday                  930 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.21 % 
Wednesday                816 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.47 % 
Thursday                 867 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Friday                   857 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.43 % 
Sunday                   1077 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.46 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 46 mins       █████████████░░░░░░░░░░░░   52.83 % 
YAML                     5 hrs 6 mins        ████████░░░░░░░░░░░░░░░░░   30.78 % 
Markdown                 56 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.71 % 
Bash                     54 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.51 % 
Docker                   19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.01 % 

🔥 Editors: 
Zsh                      8 hrs 46 mins       █████████████░░░░░░░░░░░░   52.83 % 
VS Code                  6 hrs 54 mins       ██████████░░░░░░░░░░░░░░░   41.66 % 
Obsidian                 50 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.11 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.40 % 

💻 Operating System: 
Linux                    16 hrs 35 mins      █████████████████████████   100.00 % 
```


 Last Updated on 17/08/2024 00:42:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
