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
🌞 Morning                1809 commits        ███████░░░░░░░░░░░░░░░░░░   26.16 % 
🌆 Daytime                2891 commits        ██████████░░░░░░░░░░░░░░░   41.80 % 
🌃 Evening                1959 commits        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.72 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       5 hrs 28 mins       ███████████████░░░░░░░░░░   59.24 % 
YAML                     2 hrs 47 mins       ████████░░░░░░░░░░░░░░░░░   30.17 % 
XML                      27 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.01 % 
Markdown                 24 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.45 % 
Git Config               5 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.97 % 

🔥 Editors: 
Zsh                      5 hrs 28 mins       ███████████████░░░░░░░░░░   59.24 % 
VS Code                  3 hrs 32 mins       ██████████░░░░░░░░░░░░░░░   38.21 % 
Obsidian                 14 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.55 % 

💻 Operating System: 
Linux                    9 hrs 15 mins       █████████████████████████   100.00 % 
```


 Last Updated on 23/03/2025 00:56:53 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
