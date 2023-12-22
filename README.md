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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C369%20hrs%2033%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1529 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3046 commits        ███████████░░░░░░░░░░░░░░   44.95 % 
🌃 Evening                1971 commits        ███████░░░░░░░░░░░░░░░░░░   29.08 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.41 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   999 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Tuesday                  877 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.94 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Thursday                 944 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.66 % 
Saturday                 999 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.74 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.22 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 4 hrs 12 mins       ████████░░░░░░░░░░░░░░░░░   32.64 % 
PHP                      2 hrs 31 mins       █████░░░░░░░░░░░░░░░░░░░░   19.60 % 
YAML                     2 hrs 14 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.43 % 
Other                    1 hr 11 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   09.20 % 
Jinja2                   1 hr 4 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.38 % 

🔥 Editors: 
VS Code                  8 hrs 55 mins       █████████████████░░░░░░░░   69.31 % 
Obsidian                 3 hrs 53 mins       ████████░░░░░░░░░░░░░░░░░   30.21 % 
Sublime Text             3 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.48 % 

💻 Operating System: 
Linux                    12 hrs 52 mins      █████████████████████████   100.00 % 
```


 Last Updated on 22/12/2023 00:10:30 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
