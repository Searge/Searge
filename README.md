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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C483%20hrs%2011%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1505 commits        ██████░░░░░░░░░░░░░░░░░░░   24.19 % 
🌆 Daytime                2703 commits        ███████████░░░░░░░░░░░░░░   43.45 % 
🌃 Evening                1768 commits        ███████░░░░░░░░░░░░░░░░░░   28.42 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.94 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   889 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  812 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Wednesday                835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.42 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.50 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.70 % 
Saturday                 985 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.83 % 
Sunday                   1008 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.20 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 11 mins       █████████░░░░░░░░░░░░░░░░   34.81 % 
sh                       5 hrs 8 mins        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
Markdown                 4 hrs 42 mins       ███████░░░░░░░░░░░░░░░░░░   26.44 % 
Other                    29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.73 % 
Bash                     23 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.16 % 

🔥 Editors: 
VS Code                  9 hrs 41 mins       ██████████████░░░░░░░░░░░   54.45 % 
Zsh                      5 hrs 8 mins        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
Vim                      2 hrs               ███░░░░░░░░░░░░░░░░░░░░░░   11.32 % 
Obsidian                 45 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.27 % 
Sublime Text             11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.03 % 

💻 Operating System: 
Linux                    17 hrs 47 mins      █████████████████████████   100.00 % 
```


 Last Updated on 12/05/2024 00:37:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
