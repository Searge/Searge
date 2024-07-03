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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C632%20hrs%2031%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1907 commits        ██████░░░░░░░░░░░░░░░░░░░   25.07 % 
🌆 Daytime                3052 commits        ██████████░░░░░░░░░░░░░░░   40.12 % 
🌃 Evening                2364 commits        ████████░░░░░░░░░░░░░░░░░   31.07 % 
🌙 Night                  285 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.75 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1055 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.87 % 
Tuesday                  934 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.28 % 
Wednesday                926 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.17 % 
Thursday                 876 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.51 % 
Friday                   865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.37 % 
Saturday                 1468 commits        █████░░░░░░░░░░░░░░░░░░░░   19.30 % 
Sunday                   1484 commits        █████░░░░░░░░░░░░░░░░░░░░   19.51 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 43 mins      ██████████████████░░░░░░░   71.19 % 
YAML                     2 hrs 33 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.03 % 
Markdown                 36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.01 % 
SSH Config               18 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.09 % 
Docker                   17 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.92 % 

🔥 Editors: 
Zsh                      10 hrs 43 mins      ██████████████████░░░░░░░   71.19 % 
VS Code                  3 hrs 40 mins       ██████░░░░░░░░░░░░░░░░░░░   24.39 % 
Obsidian                 36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.01 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.41 % 

💻 Operating System: 
Linux                    15 hrs 4 mins       █████████████████████████   100.00 % 
```


 Last Updated on 03/07/2024 00:43:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
