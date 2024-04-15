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
**I'm an Early 🐤** 

```text
🌞 Morning                1447 commits        ██████░░░░░░░░░░░░░░░░░░░   23.92 % 
🌆 Daytime                2655 commits        ███████████░░░░░░░░░░░░░░   43.88 % 
🌃 Evening                1707 commits        ███████░░░░░░░░░░░░░░░░░░   28.21 % 
🌙 Night                  241 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.98 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   860 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.21 % 
Tuesday                  794 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.12 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.31 % 
Thursday                 828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.69 % 
Friday                   836 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.82 % 
Saturday                 957 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.82 % 
Sunday                   970 commits         ████░░░░░░░░░░░░░░░░░░░░░   16.03 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 34 mins       ███████████████░░░░░░░░░░   60.22 % 
Other                    35 mins             ███░░░░░░░░░░░░░░░░░░░░░░   13.69 % 
Bash                     17 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.75 % 
gitrebase                13 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.19 % 
XML                      11 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.39 % 

🔥 Editors: 
VS Code                  2 hrs 27 mins       ██████████████░░░░░░░░░░░   57.56 % 
Obsidian                 1 hr 32 mins        █████████░░░░░░░░░░░░░░░░   36.09 % 
Vim                      16 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.35 % 

💻 Operating System: 
Linux                    4 hrs 15 mins       █████████████████████████   100.00 % 
```


 Last Updated on 15/04/2024 02:46:38 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
