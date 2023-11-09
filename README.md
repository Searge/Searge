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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C313%20hrs%2054%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1490 commits        ██████░░░░░░░░░░░░░░░░░░░   22.52 % 
🌆 Daytime                2974 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                1923 commits        ███████░░░░░░░░░░░░░░░░░░   29.07 % 
🌙 Night                  228 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.45 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   973 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.71 % 
Tuesday                  851 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.73 % 
Thursday                 927 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.01 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.85 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.86 % 
Sunday                   1189 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.97 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 26 mins       ███████░░░░░░░░░░░░░░░░░░   28.61 % 
Other                    2 hrs 59 mins       ██████░░░░░░░░░░░░░░░░░░░   24.81 % 
YAML                     1 hr 47 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.95 % 
conf                     48 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.70 % 
Jinja2                   35 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.87 % 

🔥 Editors: 
VS Code                  6 hrs 19 mins       █████████████░░░░░░░░░░░░   52.57 % 
Obsidian                 3 hrs 11 mins       ███████░░░░░░░░░░░░░░░░░░   26.55 % 
Vim                      2 hrs 19 mins       █████░░░░░░░░░░░░░░░░░░░░   19.35 % 
Neovim                   11 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.53 % 

💻 Operating System: 
Linux                    12 hrs 1 min        █████████████████████████   100.00 % 
```


 Last Updated on 09/11/2023 00:09:32 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
