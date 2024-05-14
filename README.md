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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C488%20hrs%2020%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1505 commits        ██████░░░░░░░░░░░░░░░░░░░   24.18 % 
🌆 Daytime                2703 commits        ███████████░░░░░░░░░░░░░░   43.42 % 
🌃 Evening                1768 commits        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
🌙 Night                  249 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   04.00 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   889 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.28 % 
Tuesday                  812 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.04 % 
Wednesday                835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.49 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.69 % 
Saturday                 985 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.82 % 
Sunday                   1012 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.26 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 5 hrs 42 mins       █████████░░░░░░░░░░░░░░░░   35.42 % 
YAML                     5 hrs 32 mins       █████████░░░░░░░░░░░░░░░░   34.36 % 
sh                       3 hrs 44 mins       ██████░░░░░░░░░░░░░░░░░░░   23.18 % 
Other                    15 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.57 % 
Bash                     12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.28 % 

🔥 Editors: 
VS Code                  9 hrs 45 mins       ███████████████░░░░░░░░░░   60.43 % 
Zsh                      3 hrs 44 mins       ██████░░░░░░░░░░░░░░░░░░░   23.18 % 
Vim                      1 hr 52 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.57 % 
Obsidian                 35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.68 % 
Sublime Text             11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.14 % 

💻 Operating System: 
Linux                    16 hrs 8 mins       █████████████████████████   100.00 % 
```


 Last Updated on 14/05/2024 00:40:45 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
