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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C174%20hrs%2018%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1268 commits        ██████░░░░░░░░░░░░░░░░░░░   22.85 % 
🌆 Daytime                2502 commits        ███████████░░░░░░░░░░░░░░   45.08 % 
🌃 Evening                1559 commits        ███████░░░░░░░░░░░░░░░░░░   28.09 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.98 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.18 % 
Tuesday                  742 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.37 % 
Wednesday                743 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.39 % 
Thursday                 785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.14 % 
Friday                   803 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.47 % 
Saturday                 854 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.39 % 
Sunday                   836 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.06 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 11 mins       ███████████████████████░░   90.40 % 
YAML                     9 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   06.62 % 
Bash                     3 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.32 % 
PHP                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.21 % 
Other                    0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.17 % 

🔥 Editors: 
Obsidian                 1 hr 55 mins        ████████████████████░░░░░   79.12 % 
VS Code                  25 mins             ████░░░░░░░░░░░░░░░░░░░░░   17.70 % 
Vim                      4 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.17 % 

💻 Operating System: 
Windows                  1 hr 36 mins        ████████████████░░░░░░░░░   65.96 % 
Linux                    49 mins             █████████░░░░░░░░░░░░░░░░   34.04 % 
```


 Last Updated on 10/08/2023 00:10:08 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
