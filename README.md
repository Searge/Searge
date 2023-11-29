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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C338%20hrs%204%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1502 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3000 commits        ███████████░░░░░░░░░░░░░░   45.05 % 
🌃 Evening                1928 commits        ███████░░░░░░░░░░░░░░░░░░   28.95 % 
🌙 Night                  229 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.44 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   980 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Tuesday                  855 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.84 % 
Wednesday                842 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.64 % 
Thursday                 928 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.94 % 
Friday                   850 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.76 % 
Saturday                 984 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
Sunday                   1220 commits        █████░░░░░░░░░░░░░░░░░░░░   18.32 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Other                    3 hrs 21 mins       ██████████░░░░░░░░░░░░░░░   39.33 % 
Markdown                 1 hr 58 mins        ██████░░░░░░░░░░░░░░░░░░░   23.17 % 
INI                      58 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.33 % 
YAML                     41 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.03 % 
Bash                     33 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.51 % 

🔥 Editors: 
VS Code                  6 hrs 41 mins       ████████████████████░░░░░   78.16 % 
Obsidian                 1 hr 51 mins        █████░░░░░░░░░░░░░░░░░░░░   21.76 % 
Vim                      0 secs              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.08 % 

💻 Operating System: 
Linux                    8 hrs 33 mins       █████████████████████████   100.00 % 
```


 Last Updated on 29/11/2023 00:10:12 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
