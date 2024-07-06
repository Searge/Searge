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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C643%20hrs%2058%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1916 commits        ██████░░░░░░░░░░░░░░░░░░░   25.08 % 
🌆 Daytime                3069 commits        ██████████░░░░░░░░░░░░░░░   40.17 % 
🌃 Evening                2370 commits        ████████░░░░░░░░░░░░░░░░░   31.02 % 
🌙 Night                  285 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.73 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1067 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.97 % 
Tuesday                  946 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.38 % 
Wednesday                927 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.13 % 
Thursday                 882 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.54 % 
Friday                   866 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.34 % 
Saturday                 1468 commits        █████░░░░░░░░░░░░░░░░░░░░   19.21 % 
Sunday                   1484 commits        █████░░░░░░░░░░░░░░░░░░░░   19.42 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 33 mins      ████████████████░░░░░░░░░   64.94 % 
YAML                     3 hrs 28 mins       █████░░░░░░░░░░░░░░░░░░░░   19.54 % 
Markdown                 1 hr 31 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.54 % 
SSH Config               18 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.77 % 
INI                      13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.23 % 

🔥 Editors: 
Zsh                      11 hrs 33 mins      ████████████████░░░░░░░░░   64.94 % 
VS Code                  4 hrs 58 mins       ███████░░░░░░░░░░░░░░░░░░   27.93 % 
Obsidian                 1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   06.62 % 
Vim                      5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.50 % 

💻 Operating System: 
Linux                    17 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 06/07/2024 00:39:26 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
