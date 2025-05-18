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
🌞 Morning                1848 commits        ███████░░░░░░░░░░░░░░░░░░   26.03 % 
🌆 Daytime                2956 commits        ██████████░░░░░░░░░░░░░░░   41.63 % 
🌃 Evening                2039 commits        ███████░░░░░░░░░░░░░░░░░░   28.72 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.62 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       11 hrs 22 mins      ████████████░░░░░░░░░░░░░   47.47 % 
YAML                     5 hrs 6 mins        █████░░░░░░░░░░░░░░░░░░░░   21.32 % 
Markdown                 2 hrs 40 mins       ███░░░░░░░░░░░░░░░░░░░░░░   11.18 % 
Python                   1 hr 59 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.31 % 
Bash                     52 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.62 % 

🔥 Editors: 
VS Code                  11 hrs 33 mins      ████████████░░░░░░░░░░░░░   48.17 % 
Zsh                      11 hrs 22 mins      ████████████░░░░░░░░░░░░░   47.47 % 
Obsidian                 1 hr 1 min          █░░░░░░░░░░░░░░░░░░░░░░░░   04.26 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.09 % 

💻 Operating System: 
Linux                    23 hrs 58 mins      █████████████████████████   100.00 % 
```


 Last Updated on 18/05/2025 00:07:36 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
