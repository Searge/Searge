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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C287%20hrs%2032%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1464 commits        ██████░░░░░░░░░░░░░░░░░░░   22.30 % 
🌆 Daytime                2958 commits        ███████████░░░░░░░░░░░░░░   45.06 % 
🌃 Evening                1915 commits        ███████░░░░░░░░░░░░░░░░░░   29.17 % 
🌙 Night                  227 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.46 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   959 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.61 % 
Tuesday                  839 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.83 % 
Thursday                 924 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.08 % 
Friday                   830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.64 % 
Saturday                 983 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.98 % 
Sunday                   1187 commits        █████░░░░░░░░░░░░░░░░░░░░   18.08 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Terraform                2 hrs 36 mins       █████░░░░░░░░░░░░░░░░░░░░   20.14 % 
GDScript                 2 hrs 2 mins        ████░░░░░░░░░░░░░░░░░░░░░   15.68 % 
YAML                     1 hr 49 mins        ████░░░░░░░░░░░░░░░░░░░░░   14.11 % 
Markdown                 1 hr 38 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.62 % 
Docker                   49 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.34 % 

🔥 Editors: 
VS Code                  10 hrs 56 mins      █████████████████████░░░░   84.33 % 
Obsidian                 1 hr 1 min          ██░░░░░░░░░░░░░░░░░░░░░░░   07.92 % 
Vim                      51 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.64 % 
Sublime Text             8 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.11 % 

💻 Operating System: 
Linux                    12 hrs 58 mins      █████████████████████████   100.00 % 
```


 Last Updated on 20/10/2023 00:09:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
