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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C384%20hrs%2059%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1516 commits        ██████░░░░░░░░░░░░░░░░░░░   22.58 % 
🌆 Daytime                3021 commits        ███████████░░░░░░░░░░░░░░   44.99 % 
🌃 Evening                1947 commits        ███████░░░░░░░░░░░░░░░░░░   28.99 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   995 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.82 % 
Tuesday                  877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.06 % 
Wednesday                858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Thursday                 935 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.92 % 
Friday                   852 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.69 % 
Saturday                 990 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Sunday                   1208 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.99 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 5 hrs 31 mins       ██████████████░░░░░░░░░░░   55.52 % 
YAML                     1 hr 53 mins        █████░░░░░░░░░░░░░░░░░░░░   19.02 % 
PHP                      48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.13 % 
Other                    45 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.68 % 
Git                      21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.68 % 

🔥 Editors: 
VS Code                  5 hrs 28 mins       ██████████████░░░░░░░░░░░   54.91 % 
Obsidian                 4 hrs 1 min         ██████████░░░░░░░░░░░░░░░   40.34 % 
Vim                      28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.75 % 

💻 Operating System: 
Linux                    8 hrs 55 mins       ██████████████████████░░░   89.70 % 
Windows                  1 hr 1 min          ███░░░░░░░░░░░░░░░░░░░░░░   10.30 % 
```


 Last Updated on 02/01/2024 00:10:46 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
