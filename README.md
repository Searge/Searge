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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C395%20hrs%2014%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1492 commits        ██████░░░░░░░░░░░░░░░░░░░   22.69 % 
🌆 Daytime                2959 commits        ███████████░░░░░░░░░░░░░░   44.99 % 
🌃 Evening                1895 commits        ███████░░░░░░░░░░░░░░░░░░   28.81 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.51 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   977 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.85 % 
Tuesday                  873 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.27 % 
Wednesday                846 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.86 % 
Thursday                 915 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.91 % 
Friday                   840 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.77 % 
Saturday                 972 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
Sunday                   1154 commits        ████░░░░░░░░░░░░░░░░░░░░░   17.55 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 3 hrs 43 mins       ███████████░░░░░░░░░░░░░░   45.98 % 
YAML                     1 hr 54 mins        ██████░░░░░░░░░░░░░░░░░░░   23.58 % 
Docker                   37 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.79 % 
Bash                     31 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.40 % 
PHP                      29 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.14 % 

🔥 Editors: 
VS Code                  4 hrs 26 mins       ██████████████░░░░░░░░░░░   54.73 % 
Obsidian                 3 hrs 32 mins       ███████████░░░░░░░░░░░░░░   43.76 % 
Vim                      7 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   01.51 % 

💻 Operating System: 
Linux                    8 hrs 4 mins        █████████████████████████   99.52 % 
Windows                  2 mins              ░░░░░░░░░░░░░░░░░░░░░░░░░   00.48 % 
```


 Last Updated on 11/01/2024 00:10:06 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
