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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C410%20hrs%2055%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1542 commits        ██████░░░░░░░░░░░░░░░░░░░   22.69 % 
🌆 Daytime                3042 commits        ███████████░░░░░░░░░░░░░░   44.76 % 
🌃 Evening                1973 commits        ███████░░░░░░░░░░░░░░░░░░   29.03 % 
🌙 Night                  239 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.52 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1007 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.82 % 
Tuesday                  903 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.29 % 
Wednesday                879 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.93 % 
Thursday                 943 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.88 % 
Friday                   854 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.57 % 
Saturday                 998 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.69 % 
Sunday                   1212 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.83 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 6 mins        ███████████░░░░░░░░░░░░░░   45.22 % 
Bash                     1 hr 19 mins        ███████░░░░░░░░░░░░░░░░░░   28.56 % 
Other                    37 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.50 % 
YAML                     15 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.64 % 
JSON                     7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.86 % 

🔥 Editors: 
VS Code                  2 hrs 16 mins       ████████████░░░░░░░░░░░░░   48.96 % 
Obsidian                 2 hrs 2 mins        ███████████░░░░░░░░░░░░░░   43.97 % 
Vim                      19 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.07 % 

💻 Operating System: 
Linux                    4 hrs 39 mins       █████████████████████████   100.00 % 
```


 Last Updated on 01/02/2024 00:10:32 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
