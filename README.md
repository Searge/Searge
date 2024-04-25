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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C457%20hrs%2026%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1484 commits        ██████░░░░░░░░░░░░░░░░░░░   24.08 % 
🌆 Daytime                2683 commits        ███████████░░░░░░░░░░░░░░   43.54 % 
🌃 Evening                1750 commits        ███████░░░░░░░░░░░░░░░░░░   28.40 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.98 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   880 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.28 % 
Tuesday                  810 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Wednesday                814 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.21 % 
Thursday                 837 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.58 % 
Friday                   842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.66 % 
Saturday                 978 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.87 % 
Sunday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.24 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 11 mins       ████████████████░░░░░░░░░   65.07 % 
YAML                     35 mins             ████░░░░░░░░░░░░░░░░░░░░░   17.77 % 
Config                   20 mins             ███░░░░░░░░░░░░░░░░░░░░░░   10.23 % 
Jinja2                   5 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.87 % 
Bash                     2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.15 % 

🔥 Editors: 
Obsidian                 1 hr 54 mins        ██████████████░░░░░░░░░░░   56.99 % 
VS Code                  1 hr 25 mins        ███████████░░░░░░░░░░░░░░   42.21 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.80 % 

💻 Operating System: 
Linux                    3 hrs 19 mins       █████████████████████████   98.89 % 
Windows                  2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.11 % 
```


 Last Updated on 25/04/2024 00:37:56 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
