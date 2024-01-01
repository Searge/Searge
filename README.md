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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C380%20hrs%2055%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1531 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3051 commits        ███████████░░░░░░░░░░░░░░   44.96 % 
🌃 Evening                1973 commits        ███████░░░░░░░░░░░░░░░░░░   29.07 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.40 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   1003 commits        ████░░░░░░░░░░░░░░░░░░░░░   14.78 % 
Tuesday                  881 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.98 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.75 % 
Thursday                 945 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.64 % 
Saturday                 999 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.72 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.20 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr 53 mins        ███████░░░░░░░░░░░░░░░░░░   29.99 % 
Markdown                 1 hr 53 mins        ███████░░░░░░░░░░░░░░░░░░   29.87 % 
PHP                      48 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.82 % 
Other                    45 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.10 % 
Git                      21 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   05.80 % 

🔥 Editors: 
VS Code                  4 hrs 35 mins       ██████████████████░░░░░░░   72.62 % 
Obsidian                 1 hr 15 mins        █████░░░░░░░░░░░░░░░░░░░░   19.89 % 
Vim                      28 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.49 % 

💻 Operating System: 
Linux                    6 hrs 18 mins       █████████████████████████   100.00 % 
```


 Last Updated on 01/01/2024 00:10:50 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
