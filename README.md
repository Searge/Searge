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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C411%20hrs%2050%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1541 commits        ██████░░░░░░░░░░░░░░░░░░░   22.77 % 
🌆 Daytime                3032 commits        ███████████░░░░░░░░░░░░░░   44.79 % 
🌃 Evening                1963 commits        ███████░░░░░░░░░░░░░░░░░░   29.00 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.79 % 
Tuesday                  899 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.28 % 
Wednesday                879 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.99 % 
Thursday                 942 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.92 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.62 % 
Saturday                 996 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Sunday                   1198 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.70 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 38 mins       █████████████░░░░░░░░░░░░   50.59 % 
Bash                     1 hr 19 mins        ██████░░░░░░░░░░░░░░░░░░░   25.39 % 
Other                    37 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.00 % 
YAML                     16 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.40 % 
JSON                     7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.54 % 

🔥 Editors: 
VS Code                  3 hrs 10 mins       ███████████████░░░░░░░░░░   60.61 % 
Obsidian                 1 hr 43 mins        ████████░░░░░░░░░░░░░░░░░   33.10 % 
Vim                      19 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.29 % 

💻 Operating System: 
Linux                    5 hrs 14 mins       █████████████████████████   100.00 % 
```


 Last Updated on 02/02/2024 00:09:27 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
