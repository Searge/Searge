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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C589%20hrs%2048%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1502 commits        ██████░░░░░░░░░░░░░░░░░░░   24.13 % 
🌆 Daytime                2700 commits        ███████████░░░░░░░░░░░░░░   43.38 % 
🌃 Evening                1783 commits        ███████░░░░░░░░░░░░░░░░░░   28.65 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   907 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.57 % 
Tuesday                  850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Wednesday                789 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.68 % 
Thursday                 830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.34 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.03 % 
Sunday                   1024 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.45 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 47 mins       ████████████████░░░░░░░░░   65.25 % 
Bash                     1 hr 29 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.54 % 
YAML                     51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.17 % 
XML                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.95 % 
XSLT                     17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.49 % 

🔥 Editors: 
Zsh                      7 hrs 47 mins       ████████████████░░░░░░░░░   65.25 % 
VS Code                  3 hrs 24 mins       ███████░░░░░░░░░░░░░░░░░░   28.59 % 
Vim                      32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.59 % 
Obsidian                 11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.57 % 

💻 Operating System: 
Linux                    11 hrs 56 mins      █████████████████████████   100.00 % 
```


 Last Updated on 15/06/2024 00:43:21 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
