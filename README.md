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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C153%20hrs%208%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1229 commits        ██████░░░░░░░░░░░░░░░░░░░   22.39 % 
🌆 Daytime                2465 commits        ███████████░░░░░░░░░░░░░░   44.90 % 
🌃 Evening                1586 commits        ███████░░░░░░░░░░░░░░░░░░   28.89 % 
🌙 Night                  210 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.83 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   787 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.34 % 
Tuesday                  737 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.42 % 
Wednesday                718 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.08 % 
Thursday                 781 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.23 % 
Friday                   785 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.30 % 
Saturday                 849 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.46 % 
Sunday                   833 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.17 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 40 mins       ███████████░░░░░░░░░░░░░░   44.64 % 
YAML                     2 hrs 34 mins       ████████░░░░░░░░░░░░░░░░░   31.34 % 
Bash                     43 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.84 % 
Other                    42 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.54 % 
INI                      14 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.87 % 

🔥 Editors: 
VS Code                  4 hrs 28 mins       ██████████████░░░░░░░░░░░   54.40 % 
Obsidian                 3 hrs 31 mins       ███████████░░░░░░░░░░░░░░   42.98 % 
Vim                      12 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.62 % 

💻 Operating System: 
Linux                    8 hrs 13 mins       █████████████████████████   100.00 % 
```


 Last Updated on 22/07/2023 00:09:30 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
