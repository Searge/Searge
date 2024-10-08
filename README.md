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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C815%20hrs%2037%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1646 commits        ██████░░░░░░░░░░░░░░░░░░░   24.96 % 
🌆 Daytime                2843 commits        ███████████░░░░░░░░░░░░░░   43.11 % 
🌃 Evening                1857 commits        ███████░░░░░░░░░░░░░░░░░░   28.16 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.76 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   978 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.83 % 
Tuesday                  933 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.15 % 
Wednesday                841 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Thursday                 883 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.25 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.38 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.24 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 19 mins      ███████████░░░░░░░░░░░░░░   45.15 % 
YAML                     8 hrs 31 mins       █████████░░░░░░░░░░░░░░░░   37.27 % 
Markdown                 2 hrs 38 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.57 % 
Docker                   26 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.96 % 
Other                    15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.09 % 

🔥 Editors: 
VS Code                  11 hrs 31 mins      █████████████░░░░░░░░░░░░   50.44 % 
Zsh                      10 hrs 19 mins      ███████████░░░░░░░░░░░░░░   45.15 % 
Obsidian                 58 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.24 % 
Vim                      2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.18 % 

💻 Operating System: 
Linux                    22 hrs 51 mins      █████████████████████████   100.00 % 
```


 Last Updated on 08/10/2024 00:51:58 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
