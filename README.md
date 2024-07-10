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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C646%20hrs%2014%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1573 commits        ██████░░░░░░░░░░░░░░░░░░░   24.58 % 
🌆 Daytime                2770 commits        ███████████░░░░░░░░░░░░░░   43.28 % 
🌃 Evening                1816 commits        ███████░░░░░░░░░░░░░░░░░░   28.38 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.77 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   948 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.81 % 
Tuesday                  894 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.97 % 
Wednesday                792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.38 % 
Thursday                 843 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.17 % 
Friday                   833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.02 % 
Saturday                 1019 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.92 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.73 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 54 mins      █████████████████░░░░░░░░   67.15 % 
YAML                     3 hrs 32 mins       █████░░░░░░░░░░░░░░░░░░░░   21.84 % 
Markdown                 1 hr 17 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.92 % 
Other                    14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.45 % 
Diff                     9 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.00 % 

🔥 Editors: 
Zsh                      10 hrs 54 mins      █████████████████░░░░░░░░   67.15 % 
VS Code                  4 hrs 17 mins       ███████░░░░░░░░░░░░░░░░░░   26.48 % 
Obsidian                 56 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.79 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.58 % 

💻 Operating System: 
Linux                    16 hrs 14 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/07/2024 00:44:04 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
