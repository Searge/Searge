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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C266%20hrs%2051%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1436 commits        ██████░░░░░░░░░░░░░░░░░░░   22.43 % 
🌆 Daytime                2884 commits        ███████████░░░░░░░░░░░░░░   45.05 % 
🌃 Evening                1855 commits        ███████░░░░░░░░░░░░░░░░░░   28.98 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.55 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   933 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.57 % 
Tuesday                  817 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Wednesday                828 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.93 % 
Thursday                 902 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Friday                   824 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.87 % 
Saturday                 965 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.07 % 
Sunday                   1133 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.70 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 7 hrs 46 mins       █████████████░░░░░░░░░░░░   50.57 % 
YAML                     3 hrs 16 mins       █████░░░░░░░░░░░░░░░░░░░░   21.35 % 
Bash                     1 hr 53 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.36 % 
Docker                   1 hr 10 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.63 % 
Ezhil                    28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.07 % 

🔥 Editors: 
VS Code                  7 hrs 59 mins       █████████████░░░░░░░░░░░░   52.00 % 
Obsidian                 7 hrs 20 mins       ████████████░░░░░░░░░░░░░   47.72 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.15 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.12 % 

💻 Operating System: 
Linux                    15 hrs 22 mins      █████████████████████████   100.00 % 
```


 Last Updated on 12/10/2023 00:09:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
