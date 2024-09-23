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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C781%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1656 commits        ██████░░░░░░░░░░░░░░░░░░░   25.12 % 
🌆 Daytime                2832 commits        ███████████░░░░░░░░░░░░░░   42.95 % 
🌃 Evening                1857 commits        ███████░░░░░░░░░░░░░░░░░░   28.17 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.76 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   965 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.64 % 
Tuesday                  926 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.05 % 
Wednesday                846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.83 % 
Thursday                 882 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.38 % 
Friday                   877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.30 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.24 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     9 hrs 36 mins       ████████████░░░░░░░░░░░░░   48.27 % 
sh                       8 hrs 33 mins       ███████████░░░░░░░░░░░░░░   43.00 % 
Other                    1 hr 2 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.23 % 
DNS Zone                 12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.02 % 
Bash                     9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.78 % 

🔥 Editors: 
VS Code                  11 hrs 15 mins      ██████████████░░░░░░░░░░░   56.62 % 
Zsh                      8 hrs 33 mins       ███████████░░░░░░░░░░░░░░   43.00 % 
Obsidian                 2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.21 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.18 % 

💻 Operating System: 
Linux                    19 hrs 53 mins      █████████████████████████   100.00 % 
```


 Last Updated on 23/09/2024 00:50:14 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
