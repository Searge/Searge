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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C664%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1584 commits        ██████░░░░░░░░░░░░░░░░░░░   24.60 % 
🌆 Daytime                2786 commits        ███████████░░░░░░░░░░░░░░   43.27 % 
🌃 Evening                1824 commits        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.79 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   958 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.88 % 
Tuesday                  898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.95 % 
Wednesday                809 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Thursday                 852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.23 % 
Friday                   839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.03 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.69 % 
Sunday                   1072 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.65 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 45 mins       ██████████████████░░░░░░░   73.11 % 
YAML                     1 hr 27 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.93 % 
Markdown                 1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.77 % 
Text                     16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.11 % 
Other                    15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.93 % 

🔥 Editors: 
Zsh                      9 hrs 45 mins       ██████████████████░░░░░░░   73.11 % 
VS Code                  2 hrs 5 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.65 % 
Obsidian                 1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.77 % 
Vim                      19 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.47 % 

💻 Operating System: 
Linux                    13 hrs 20 mins      █████████████████████████   100.00 % 
```


 Last Updated on 18/07/2024 00:43:14 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
