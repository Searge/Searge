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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C387%20hrs%2023%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1492 commits        ██████░░░░░░░░░░░░░░░░░░░   22.69 % 
🌆 Daytime                2959 commits        ███████████░░░░░░░░░░░░░░   44.99 % 
🌃 Evening                1895 commits        ███████░░░░░░░░░░░░░░░░░░   28.81 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.51 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.85 % 
Tuesday                  873 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Wednesday                846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Thursday                 915 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.91 % 
Friday                   840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Saturday                 972 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
Sunday                   1154 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.55 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 6 hrs 6 mins        ████████████████████████░   94.25 % 
Bash                     7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.97 % 
YAML                     7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.94 % 
sh                       3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.85 % 
Docker                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.40 % 

🔥 Editors: 
Obsidian                 5 hrs 9 mins        ████████████████████░░░░░   79.39 % 
VS Code                  1 hr 16 mins        █████░░░░░░░░░░░░░░░░░░░░   19.68 % 
Vim                      3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.93 % 

💻 Operating System: 
Linux                    4 hrs 39 mins       ██████████████████░░░░░░░   71.79 % 
Windows                  1 hr 49 mins        ███████░░░░░░░░░░░░░░░░░░   28.21 % 
```


 Last Updated on 06/01/2024 00:09:31 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
