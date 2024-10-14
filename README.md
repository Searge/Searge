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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C834%20hrs%203%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1639 commits        ██████░░░░░░░░░░░░░░░░░░░   25.13 % 
🌆 Daytime                2794 commits        ███████████░░░░░░░░░░░░░░   42.84 % 
🌃 Evening                1841 commits        ███████░░░░░░░░░░░░░░░░░░   28.23 % 
🌙 Night                  248 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.80 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   938 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.38 % 
Tuesday                  893 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.69 % 
Wednesday                853 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.08 % 
Thursday                 874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Friday                   874 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.40 % 
Saturday                 1014 commits        ████░░░░░░░░░░░░░░░░░░░░░   15.55 % 
Sunday                   1076 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.50 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       10 hrs 23 mins      █████████████░░░░░░░░░░░░   52.90 % 
YAML                     6 hrs 51 mins       █████████░░░░░░░░░░░░░░░░   34.92 % 
DNS Zone                 54 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.59 % 
Markdown                 37 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.21 % 
Other                    35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.98 % 

🔥 Editors: 
Zsh                      10 hrs 23 mins      █████████████░░░░░░░░░░░░   52.90 % 
VS Code                  8 hrs 29 mins       ███████████░░░░░░░░░░░░░░   43.30 % 
Obsidian                 23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.02 % 
Vim                      21 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.78 % 

💻 Operating System: 
Linux                    19 hrs 37 mins      █████████████████████████   100.00 % 
```


 Last Updated on 14/10/2024 00:51:05 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
