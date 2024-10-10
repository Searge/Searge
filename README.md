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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C825%20hrs%2057%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1657 commits        ██████░░░░░░░░░░░░░░░░░░░   25.08 % 
🌆 Daytime                2844 commits        ███████████░░░░░░░░░░░░░░   43.05 % 
🌃 Evening                1857 commits        ███████░░░░░░░░░░░░░░░░░░   28.11 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   978 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.80 % 
Tuesday                  933 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.12 % 
Wednesday                853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.91 % 
Thursday                 883 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.35 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 51 mins      ████████████░░░░░░░░░░░░░   49.69 % 
YAML                     7 hrs 41 mins       █████████░░░░░░░░░░░░░░░░   35.20 % 
Markdown                 1 hr 41 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.74 % 
Docker                   26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.05 % 
Other                    24 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.87 % 

🔥 Editors: 
Zsh                      10 hrs 51 mins      ████████████░░░░░░░░░░░░░   49.69 % 
VS Code                  10 hrs 13 mins      ████████████░░░░░░░░░░░░░   46.83 % 
Obsidian                 33 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.53 % 
Vim                      12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.96 % 

💻 Operating System: 
Linux                    21 hrs 50 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/10/2024 00:52:11 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
