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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C317%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1507 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3010 commits        ███████████░░░░░░░░░░░░░░   45.07 % 
🌃 Evening                1932 commits        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
🌙 Night                  230 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   981 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.69 % 
Tuesday                  855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.80 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.61 % 
Thursday                 928 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.89 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.73 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Sunday                   1240 commits        █████░░░░░░░░░░░░░░░░░░░░   18.57 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Other                    2 hrs 29 mins       █████████░░░░░░░░░░░░░░░░   35.66 % 
Markdown                 1 hr 51 mins        ███████░░░░░░░░░░░░░░░░░░   26.56 % 
VCL                      1 hr 24 mins        █████░░░░░░░░░░░░░░░░░░░░   20.13 % 
zsh                      20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.88 % 
YAML                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.77 % 

🔥 Editors: 
VS Code                  4 hrs 18 mins       ███████████████░░░░░░░░░░   61.52 % 
Obsidian                 1 hr 50 mins        ███████░░░░░░░░░░░░░░░░░░   26.28 % 
Vim                      36 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.59 % 
Neovim                   11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.63 % 
Sublime Text             4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.97 % 

💻 Operating System: 
Linux                    6 hrs 59 mins       █████████████████████████   100.00 % 
```


 Last Updated on 13/11/2023 00:09:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
