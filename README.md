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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C026%20hrs%2011%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1704 commits        ██████░░░░░░░░░░░░░░░░░░░   25.35 % 
🌆 Daytime                2847 commits        ███████████░░░░░░░░░░░░░░   42.35 % 
🌃 Evening                1914 commits        ███████░░░░░░░░░░░░░░░░░░   28.47 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.82 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       6 hrs 40 mins       ███████████░░░░░░░░░░░░░░   42.61 % 
Markdown                 4 hrs 4 mins        ███████░░░░░░░░░░░░░░░░░░   26.07 % 
Go                       1 hr 23 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.91 % 
YAML                     1 hr 13 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.77 % 
Emacs Lisp               32 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.49 % 

🔥 Editors: 
VS Code                  7 hrs 32 mins       ████████████░░░░░░░░░░░░░   48.15 % 
Zsh                      6 hrs 40 mins       ███████████░░░░░░░░░░░░░░   42.61 % 
Obsidian                 1 hr 18 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.35 % 
Vim                      6 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.70 % 
Cursor                   1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.18 % 

💻 Operating System: 
Linux                    15 hrs 39 mins      █████████████████████████   100.00 % 
```


 Last Updated on 22/12/2024 00:50:28 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
