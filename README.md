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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C187%20hrs%2039%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1799 commits        ███████░░░░░░░░░░░░░░░░░░   26.19 % 
🌆 Daytime                2864 commits        ██████████░░░░░░░░░░░░░░░   41.69 % 
🌃 Evening                1949 commits        ███████░░░░░░░░░░░░░░░░░░   28.37 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.74 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     8 hrs 26 mins       █████████░░░░░░░░░░░░░░░░   34.70 % 
sh                       7 hrs 36 mins       ████████░░░░░░░░░░░░░░░░░   31.28 % 
Markdown                 4 hrs 14 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.42 % 
HTML                     2 hrs 2 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   08.36 % 
Python                   37 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.55 % 

🔥 Editors: 
VS Code                  15 hrs 39 mins      ████████████████░░░░░░░░░   64.32 % 
Zsh                      7 hrs 36 mins       ████████░░░░░░░░░░░░░░░░░   31.28 % 
Obsidian                 49 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   03.37 % 
Sublime Text             14 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.03 % 

💻 Operating System: 
Linux                    24 hrs 19 mins      █████████████████████████   100.00 % 
```


 Last Updated on 16/03/2025 00:53:48 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
