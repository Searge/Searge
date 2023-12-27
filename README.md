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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C376%20hrs%2026%20mins-blue)

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
YAML                     2 hrs 40 mins       █████░░░░░░░░░░░░░░░░░░░░   21.38 % 
PHP                      2 hrs 39 mins       █████░░░░░░░░░░░░░░░░░░░░   21.27 % 
Other                    2 hrs 5 mins        ████░░░░░░░░░░░░░░░░░░░░░   16.74 % 
Markdown                 1 hr 33 mins        ███░░░░░░░░░░░░░░░░░░░░░░   12.38 % 
Jinja2                   1 hr 4 mins         ██░░░░░░░░░░░░░░░░░░░░░░░   08.61 % 

🔥 Editors: 
VS Code                  10 hrs 4 mins       ████████████████████░░░░░   80.35 % 
Obsidian                 1 hr 28 mins        ███░░░░░░░░░░░░░░░░░░░░░░   11.75 % 
Sublime Text             36 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   04.92 % 
Vim                      22 mins             █░░░░░░░░░░░░░░░░░░░░░░░░   02.98 % 

💻 Operating System: 
Linux                    12 hrs 31 mins      █████████████████████████   100.00 % 
```


 Last Updated on 27/12/2023 00:09:43 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
