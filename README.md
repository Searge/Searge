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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C513%20hrs%2027%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1510 commits        ██████░░░░░░░░░░░░░░░░░░░   24.18 % 
🌆 Daytime                2717 commits        ███████████░░░░░░░░░░░░░░   43.51 % 
🌃 Evening                1768 commits        ███████░░░░░░░░░░░░░░░░░░   28.32 % 
🌙 Night                  249 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   892 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.21 % 
Wednesday                836 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Thursday                 841 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.47 % 
Friday                   853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Saturday                 985 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.78 % 
Sunday                   1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     11 hrs 12 mins      ██████████░░░░░░░░░░░░░░░   40.76 % 
sh                       10 hrs 39 mins      ██████████░░░░░░░░░░░░░░░   38.76 % 
Markdown                 1 hr 58 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.18 % 
Go                       1 hr 31 mins        █░░░░░░░░░░░░░░░░░░░░░░░░   05.57 % 
Bash                     36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.22 % 

🔥 Editors: 
VS Code                  14 hrs 47 mins      █████████████░░░░░░░░░░░░   53.83 % 
Zsh                      10 hrs 39 mins      ██████████░░░░░░░░░░░░░░░   38.76 % 
Obsidian                 1 hr 39 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.05 % 
Vim                      19 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.20 % 
Sublime Text             2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.16 % 

💻 Operating System: 
Linux                    27 hrs 29 mins      █████████████████████████   100.00 % 
```


 Last Updated on 21/05/2024 00:41:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
