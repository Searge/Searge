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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C290%20hrs%2016%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1454 commits        ██████░░░░░░░░░░░░░░░░░░░   22.58 % 
🌆 Daytime                2896 commits        ███████████░░░░░░░░░░░░░░   44.97 % 
🌃 Evening                1863 commits        ███████░░░░░░░░░░░░░░░░░░   28.93 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.52 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   941 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.61 % 
Tuesday                  831 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.90 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Thursday                 904 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.04 % 
Friday                   838 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.01 % 
Saturday                 965 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.98 % 
Sunday                   1133 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.59 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr 48 mins        █████░░░░░░░░░░░░░░░░░░░░   21.32 % 
Markdown                 1 hr 41 mins        █████░░░░░░░░░░░░░░░░░░░░   19.95 % 
GDScript                 1 hr 19 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.60 % 
Terraform                1 hr 9 mins         ███░░░░░░░░░░░░░░░░░░░░░░   13.68 % 
Docker                   49 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   09.70 % 

🔥 Editors: 
VS Code                  6 hrs 40 mins       ████████████████████░░░░░   78.66 % 
Obsidian                 1 hr 4 mins         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Vim                      35 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.88 % 
Sublime Text             8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.70 % 

💻 Operating System: 
Linux                    8 hrs 29 mins       █████████████████████████   100.00 % 
```


 Last Updated on 22/10/2023 00:10:13 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
