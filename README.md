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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C453%20hrs%2050%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1466 commits        ██████░░░░░░░░░░░░░░░░░░░   23.95 % 
🌆 Daytime                2667 commits        ███████████░░░░░░░░░░░░░░   43.57 % 
🌃 Evening                1743 commits        ███████░░░░░░░░░░░░░░░░░░   28.48 % 
🌙 Night                  245 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   04.00 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   876 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.31 % 
Tuesday                  796 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.15 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.53 % 
Friday                   837 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.67 % 
Saturday                 978 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.98 % 
Sunday                   1001 commits        ████░░░░░░░░░░░░░░░░░░░░░   16.35 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 11 mins       ██████████████░░░░░░░░░░░   56.45 % 
Other                    35 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.98 % 
Bash                     17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.38 % 
gitrebase                13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.70 % 
XML                      11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.80 % 

🔥 Editors: 
VS Code                  2 hrs 26 mins       ████████████████░░░░░░░░░   62.61 % 
Obsidian                 1 hr 11 mins        ████████░░░░░░░░░░░░░░░░░   30.42 % 
Vim                      16 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.97 % 

💻 Operating System: 
Linux                    3 hrs 53 mins       █████████████████████████   100.00 % 
```


 Last Updated on 16/04/2024 00:38:35 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
