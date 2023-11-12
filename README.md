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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C317%20hrs%2020%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1492 commits        ██████░░░░░░░░░░░░░░░░░░░   22.52 % 
🌆 Daytime                2979 commits        ███████████░░░░░░░░░░░░░░   44.97 % 
🌃 Evening                1925 commits        ███████░░░░░░░░░░░░░░░░░░   29.06 % 
🌙 Night                  228 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.75 % 
Tuesday                  855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.91 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.71 % 
Thursday                 928 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.01 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.83 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.84 % 
Sunday                   1189 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.95 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 45 mins       ███████████░░░░░░░░░░░░░░   42.35 % 
Other                    2 hrs 29 mins       ███████░░░░░░░░░░░░░░░░░░   28.09 % 
VCL                      1 hr 24 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.86 % 
zsh                      20 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.85 % 
Go                       15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.97 % 

🔥 Editors: 
VS Code                  4 hrs 17 mins       ████████████░░░░░░░░░░░░░   48.26 % 
Obsidian                 3 hrs 44 mins       ███████████░░░░░░░░░░░░░░   42.13 % 
Vim                      36 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.77 % 
Neovim                   11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.07 % 
Sublime Text             4 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.77 % 

💻 Operating System: 
Linux                    8 hrs 52 mins       █████████████████████████   100.00 % 
```


 Last Updated on 12/11/2023 00:10:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
