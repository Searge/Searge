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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C764%20hrs%204%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1658 commits        ██████░░░░░░░░░░░░░░░░░░░   25.00 % 
🌆 Daytime                2857 commits        ███████████░░░░░░░░░░░░░░   43.08 % 
🌃 Evening                1870 commits        ███████░░░░░░░░░░░░░░░░░░   28.20 % 
🌙 Night                  247 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   990 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.93 % 
Tuesday                  941 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.19 % 
Wednesday                850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Thursday                 889 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   868 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.09 % 
Saturday                 1032 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.56 % 
Sunday                   1062 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.01 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 11 mins       ██████████████░░░░░░░░░░░   55.74 % 
YAML                     4 hrs 22 mins       ███████░░░░░░░░░░░░░░░░░░   29.75 % 
Markdown                 58 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.66 % 
Terraform                26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.02 % 
Other                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.75 % 

🔥 Editors: 
Zsh                      8 hrs 11 mins       ██████████████░░░░░░░░░░░   55.74 % 
VS Code                  5 hrs 18 mins       █████████░░░░░░░░░░░░░░░░   36.17 % 
Obsidian                 53 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.05 % 
Vim                      17 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.03 % 

💻 Operating System: 
Linux                    14 hrs 41 mins      █████████████████████████   100.00 % 
```


 Last Updated on 15/09/2024 00:49:44 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
