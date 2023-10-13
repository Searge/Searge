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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C275%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1438 commits        ██████░░░░░░░░░░░░░░░░░░░   22.43 % 
🌆 Daytime                2889 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1857 commits        ███████░░░░░░░░░░░░░░░░░░   28.97 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.54 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   937 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.62 % 
Tuesday                  821 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.81 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.92 % 
Thursday                 903 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Friday                   824 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.85 % 
Saturday                 965 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.05 % 
Sunday                   1133 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.67 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 48 mins       ████████████░░░░░░░░░░░░░   47.51 % 
YAML                     2 hrs 42 mins       ████░░░░░░░░░░░░░░░░░░░░░   16.52 % 
Bash                     1 hr 45 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.67 % 
Docker                   1 hr 2 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   06.35 % 
GDScript                 43 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.38 % 

🔥 Editors: 
VS Code                  9 hrs               ██████████████░░░░░░░░░░░   54.86 % 
Obsidian                 7 hrs 22 mins       ███████████░░░░░░░░░░░░░░   44.88 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.14 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.12 % 

💻 Operating System: 
Linux                    16 hrs 25 mins      █████████████████████████   100.00 % 
```


 Last Updated on 13/10/2023 00:09:42 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
