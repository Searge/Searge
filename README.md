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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C660%20hrs%2023%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1588 commits        ██████░░░░░░░░░░░░░░░░░░░   24.65 % 
🌆 Daytime                2786 commits        ███████████░░░░░░░░░░░░░░   43.25 % 
🌃 Evening                1826 commits        ███████░░░░░░░░░░░░░░░░░░   28.35 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   964 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.97 % 
Tuesday                  898 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.94 % 
Wednesday                795 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.34 % 
Thursday                 853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Friday                   834 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.95 % 
Saturday                 1026 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.93 % 
Sunday                   1071 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.63 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       13 hrs 40 mins      ███████████████████░░░░░░   76.92 % 
YAML                     2 hrs 3 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.54 % 
Markdown                 1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.93 % 
Other                    19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.84 % 
Text                     16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.55 % 

🔥 Editors: 
Zsh                      13 hrs 40 mins      ███████████████████░░░░░░   76.92 % 
VS Code                  2 hrs 35 mins       ████░░░░░░░░░░░░░░░░░░░░░   14.58 % 
Obsidian                 1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.91 % 
Vim                      17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.60 % 

💻 Operating System: 
Linux                    17 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 16/07/2024 00:42:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
