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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C683%20hrs%2049%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1595 commits        ██████░░░░░░░░░░░░░░░░░░░   24.58 % 
🌆 Daytime                2814 commits        ███████████░░░░░░░░░░░░░░   43.36 % 
🌃 Evening                1837 commits        ███████░░░░░░░░░░░░░░░░░░   28.31 % 
🌙 Night                  244 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.76 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   970 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.95 % 
Tuesday                  909 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.01 % 
Wednesday                813 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.53 % 
Thursday                 859 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.24 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.16 % 
Saturday                 1010 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   1075 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.56 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       7 hrs 36 mins       █████████████░░░░░░░░░░░░   53.40 % 
YAML                     4 hrs 2 mins        ███████░░░░░░░░░░░░░░░░░░   28.36 % 
Markdown                 1 hr 11 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.39 % 
Smarty                   30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.55 % 
Bash                     18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.12 % 

🔥 Editors: 
Zsh                      7 hrs 36 mins       █████████████░░░░░░░░░░░░   53.40 % 
VS Code                  5 hrs 31 mins       ██████████░░░░░░░░░░░░░░░   38.82 % 
Obsidian                 1 hr 6 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   07.77 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.00 % 

💻 Operating System: 
Linux                    14 hrs 14 mins      █████████████████████████   100.00 % 
```


 Last Updated on 29/07/2024 00:42:17 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
