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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C170%20hrs%2023%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1206 commits        ██████░░░░░░░░░░░░░░░░░░░   22.58 % 
🌆 Daytime                2410 commits        ███████████░░░░░░░░░░░░░░   45.13 % 
🌃 Evening                1515 commits        ███████░░░░░░░░░░░░░░░░░░   28.37 % 
🌙 Night                  209 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.91 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   774 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.49 % 
Tuesday                  720 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.48 % 
Wednesday                684 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
Thursday                 755 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   769 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.40 % 
Saturday                 829 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.52 % 
Sunday                   809 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.15 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     5 hrs 43 mins       ███████████░░░░░░░░░░░░░░   43.32 % 
Markdown                 4 hrs 29 mins       ████████░░░░░░░░░░░░░░░░░   33.89 % 
Bash                     2 hrs 52 mins       █████░░░░░░░░░░░░░░░░░░░░   21.75 % 
Nginx                    2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.34 % 
Other                    2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.32 % 

🔥 Editors: 
VS Code                  8 hrs 50 mins       █████████████████░░░░░░░░   66.82 % 
Obsidian                 4 hrs 23 mins       ████████░░░░░░░░░░░░░░░░░   33.18 % 

💻 Operating System: 
Linux                    13 hrs 13 mins      █████████████████████████   100.00 % 
```


 Last Updated on 03/08/2023 00:09:20 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
