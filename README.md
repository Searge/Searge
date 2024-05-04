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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C464%20hrs%2035%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1501 commits        ██████░░░░░░░░░░░░░░░░░░░   24.18 % 
🌆 Daytime                2699 commits        ███████████░░░░░░░░░░░░░░   43.48 % 
🌃 Evening                1762 commits        ███████░░░░░░░░░░░░░░░░░░   28.39 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.95 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   885 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.26 % 
Tuesday                  811 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.07 % 
Wednesday                833 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.42 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.73 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.79 % 
Sunday                   1006 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.21 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     6 hrs 48 mins       ████████████████░░░░░░░░░   65.45 % 
Markdown                 2 hrs 55 mins       ███████░░░░░░░░░░░░░░░░░░   28.13 % 
Diff                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.47 % 
Bash                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.41 % 
INI                      7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.27 % 

🔥 Editors: 
VS Code                  7 hrs 35 mins       ██████████████████░░░░░░░   72.88 % 
Obsidian                 1 hr 55 mins        █████░░░░░░░░░░░░░░░░░░░░   18.48 % 
Vim                      53 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.64 % 

💻 Operating System: 
Linux                    10 hrs 24 mins      █████████████████████████   100.00 % 
```


 Last Updated on 04/05/2024 00:40:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
