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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C265%20hrs%201%20min-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1421 commits        ██████░░░░░░░░░░░░░░░░░░░   22.50 % 
🌆 Daytime                2843 commits        ███████████░░░░░░░░░░░░░░   45.01 % 
🌃 Evening                1825 commits        ███████░░░░░░░░░░░░░░░░░░   28.89 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.59 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   916 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.50 % 
Tuesday                  805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Wednesday                821 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.00 % 
Thursday                 890 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Friday                   822 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.01 % 
Saturday                 956 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.14 % 
Sunday                   1106 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.51 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 9 hrs 6 mins        ██████████████░░░░░░░░░░░   54.74 % 
YAML                     4 hrs 28 mins       ███████░░░░░░░░░░░░░░░░░░   26.90 % 
Docker                   1 hr 1 min          ██░░░░░░░░░░░░░░░░░░░░░░░   06.15 % 
Bash                     28 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.86 % 
Ezhil                    24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.49 % 

🔥 Editors: 
Obsidian                 8 hrs 44 mins       █████████████░░░░░░░░░░░░   52.52 % 
VS Code                  7 hrs 53 mins       ████████████░░░░░░░░░░░░░   47.34 % 
Neovim                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.14 % 

💻 Operating System: 
Linux                    16 hrs 39 mins      █████████████████████████   100.00 % 
```


 Last Updated on 10/10/2023 00:09:38 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
