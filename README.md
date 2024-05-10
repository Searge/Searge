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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C475%20hrs%2019%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1505 commits        ██████░░░░░░░░░░░░░░░░░░░   24.21 % 
🌆 Daytime                2699 commits        ███████████░░░░░░░░░░░░░░   43.42 % 
🌃 Evening                1767 commits        ███████░░░░░░░░░░░░░░░░░░   28.43 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.94 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   889 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.30 % 
Tuesday                  812 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.06 % 
Wednesday                835 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.43 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.51 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.71 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.77 % 
Sunday                   1008 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 33 mins       ███████████░░░░░░░░░░░░░░   43.36 % 
sh                       5 hrs 8 mins        █████████░░░░░░░░░░░░░░░░   34.03 % 
Markdown                 1 hr 31 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.06 % 
Bash                     30 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.31 % 
Other                    29 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.21 % 

🔥 Editors: 
VS Code                  7 hrs 11 mins       ████████████░░░░░░░░░░░░░   47.60 % 
Zsh                      5 hrs 8 mins        █████████░░░░░░░░░░░░░░░░   34.03 % 
Vim                      1 hr 25 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.42 % 
Obsidian                 1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.73 % 
Sublime Text             11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.22 % 

💻 Operating System: 
Linux                    15 hrs 7 mins       █████████████████████████   100.00 % 
```


 Last Updated on 10/05/2024 00:40:46 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
