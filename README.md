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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C594%20hrs%2027%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1504 commits        ██████░░░░░░░░░░░░░░░░░░░   24.16 % 
🌆 Daytime                2700 commits        ███████████░░░░░░░░░░░░░░   43.37 % 
🌃 Evening                1783 commits        ███████░░░░░░░░░░░░░░░░░░   28.64 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.84 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   907 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.57 % 
Tuesday                  850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.65 % 
Wednesday                789 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.67 % 
Thursday                 830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.33 % 
Friday                   826 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Saturday                 999 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.05 % 
Sunday                   1025 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.46 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 16 mins       ████████████████░░░░░░░░░   65.82 % 
Bash                     1 hr 32 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.93 % 
YAML                     51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.05 % 
Other                    47 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.65 % 
XML                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.19 % 

🔥 Editors: 
Zsh                      9 hrs 16 mins       ████████████████░░░░░░░░░   65.82 % 
VS Code                  4 hrs               ███████░░░░░░░░░░░░░░░░░░   28.46 % 
Vim                      35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.19 % 
Obsidian                 12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.53 % 

💻 Operating System: 
Linux                    14 hrs 5 mins       █████████████████████████   100.00 % 
```


 Last Updated on 17/06/2024 00:40:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
