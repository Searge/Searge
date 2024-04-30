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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C458%20hrs%2038%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1494 commits        ██████░░░░░░░░░░░░░░░░░░░   24.17 % 
🌆 Daytime                2689 commits        ███████████░░░░░░░░░░░░░░   43.50 % 
🌃 Evening                1754 commits        ███████░░░░░░░░░░░░░░░░░░   28.37 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.96 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   885 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.32 % 
Tuesday                  810 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.10 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.17 % 
Thursday                 840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.59 % 
Friday                   847 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.70 % 
Saturday                 980 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.85 % 
Sunday                   1006 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.27 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 1 hr 27 mins        █████████████░░░░░░░░░░░░   53.35 % 
YAML                     35 mins             █████░░░░░░░░░░░░░░░░░░░░   21.78 % 
Config                   20 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.59 % 
Other                    12 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.51 % 
Jinja2                   3 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.15 % 

🔥 Editors: 
VS Code                  1 hr 23 mins        █████████████░░░░░░░░░░░░   50.74 % 
Obsidian                 1 hr 20 mins        ████████████░░░░░░░░░░░░░   49.26 % 

💻 Operating System: 
Linux                    2 hrs 43 mins       █████████████████████████   100.00 % 
```


 Last Updated on 30/04/2024 00:40:05 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
