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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C688%20hrs%2017%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1576 commits        ██████░░░░░░░░░░░░░░░░░░░   24.42 % 
🌆 Daytime                2807 commits        ███████████░░░░░░░░░░░░░░   43.49 % 
🌃 Evening                1831 commits        ███████░░░░░░░░░░░░░░░░░░   28.37 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.73 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   971 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.04 % 
Tuesday                  906 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Wednesday                800 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.39 % 
Thursday                 853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.21 % 
Friday                   846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.11 % 
Saturday                 1005 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.57 % 
Sunday                   1074 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.64 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 22 mins       ████████████░░░░░░░░░░░░░   48.36 % 
sh                       3 hrs 37 mins       ████████░░░░░░░░░░░░░░░░░   32.58 % 
Markdown                 55 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.39 % 
Smarty                   30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.57 % 
Bash                     18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.72 % 

🔥 Editors: 
VS Code                  6 hrs 33 mins       ███████████████░░░░░░░░░░   58.98 % 
Zsh                      3 hrs 37 mins       ████████░░░░░░░░░░░░░░░░░   32.58 % 
Obsidian                 55 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.39 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.05 % 

💻 Operating System: 
Linux                    11 hrs 6 mins       █████████████████████████   100.00 % 
```


 Last Updated on 01/08/2024 00:44:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
