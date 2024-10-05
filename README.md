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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C811%20hrs%209%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1955 commits        ██████░░░░░░░░░░░░░░░░░░░   25.88 % 
🌆 Daytime                3000 commits        ██████████░░░░░░░░░░░░░░░   39.71 % 
🌃 Evening                2301 commits        ████████░░░░░░░░░░░░░░░░░   30.46 % 
🌙 Night                  298 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.94 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   1053 commits        ███░░░░░░░░░░░░░░░░░░░░░░   13.94 % 
Tuesday                  981 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.99 % 
Wednesday                923 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.22 % 
Thursday                 942 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.47 % 
Friday                   900 commits         ███░░░░░░░░░░░░░░░░░░░░░░   11.91 % 
Saturday                 1414 commits        █████░░░░░░░░░░░░░░░░░░░░   18.72 % 
Sunday                   1341 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.75 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 33 mins       ███████████░░░░░░░░░░░░░░   45.30 % 
YAML                     6 hrs 51 mins       █████████░░░░░░░░░░░░░░░░   36.37 % 
Markdown                 2 hrs 32 mins       ███░░░░░░░░░░░░░░░░░░░░░░   13.50 % 
Docker                   26 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.34 % 
Bash                     16 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.49 % 

🔥 Editors: 
VS Code                  9 hrs 5 mins        ████████████░░░░░░░░░░░░░   48.17 % 
Zsh                      8 hrs 33 mins       ███████████░░░░░░░░░░░░░░   45.30 % 
Obsidian                 1 hr 3 mins         █░░░░░░░░░░░░░░░░░░░░░░░░   05.56 % 
Vim                      10 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.96 % 

💻 Operating System: 
Linux                    18 hrs 52 mins      █████████████████████████   100.00 % 
```


 Last Updated on 05/10/2024 00:48:49 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
