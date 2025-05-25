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
![Code Time](http://img.shields.io/badge/Code%20Time-3%2C383%20hrs%2024%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1854 commits        ███████░░░░░░░░░░░░░░░░░░   26.04 % 
🌆 Daytime                2968 commits        ██████████░░░░░░░░░░░░░░░   41.69 % 
🌃 Evening                2041 commits        ███████░░░░░░░░░░░░░░░░░░   28.67 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.61 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       9 hrs 17 mins       █████████████░░░░░░░░░░░░   51.74 % 
YAML                     3 hrs 20 mins       █████░░░░░░░░░░░░░░░░░░░░   18.65 % 
Markdown                 3 hrs 17 mins       █████░░░░░░░░░░░░░░░░░░░░   18.31 % 
Other                    47 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.40 % 
Bash                     26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.46 % 

🔥 Editors: 
Zsh                      9 hrs 17 mins       █████████████░░░░░░░░░░░░   51.74 % 
VS Code                  7 hrs 23 mins       ██████████░░░░░░░░░░░░░░░   41.17 % 
Obsidian                 49 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.62 % 
Sublime Text             26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.44 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.03 % 

💻 Operating System: 
Linux                    17 hrs 57 mins      █████████████████████████   100.00 % 
```


 Last Updated on 25/05/2025 00:07:29 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
