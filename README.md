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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C096%20hrs%2029%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1729 commits        ██████░░░░░░░░░░░░░░░░░░░   25.53 % 
🌆 Daytime                2861 commits        ███████████░░░░░░░░░░░░░░   42.25 % 
🌃 Evening                1924 commits        ███████░░░░░░░░░░░░░░░░░░   28.41 % 
🌙 Night                  258 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
SCSS                     4 hrs 6 mins        ████████░░░░░░░░░░░░░░░░░   31.97 % 
sh                       4 hrs 2 mins        ████████░░░░░░░░░░░░░░░░░   31.37 % 
HTML                     1 hr 23 mins        ███░░░░░░░░░░░░░░░░░░░░░░   10.76 % 
Python                   45 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.83 % 
Markdown                 42 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.45 % 

🔥 Editors: 
VS Code                  7 hrs 57 mins       ███████████████░░░░░░░░░░   61.84 % 
Zsh                      4 hrs 2 mins        ████████░░░░░░░░░░░░░░░░░   31.37 % 
Obsidian                 38 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.00 % 
Cursor                   12 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.65 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.14 % 

💻 Operating System: 
Linux                    12 hrs 52 mins      █████████████████████████   100.00 % 
```


 Last Updated on 26/01/2025 00:51:40 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
