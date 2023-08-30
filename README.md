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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C190%20hrs%2010%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1325 commits        ██████░░░░░░░░░░░░░░░░░░░   22.82 % 
🌆 Daytime                2616 commits        ███████████░░░░░░░░░░░░░░   45.05 % 
🌃 Evening                1645 commits        ███████░░░░░░░░░░░░░░░░░░   28.33 % 
🌙 Night                  221 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.81 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   818 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.09 % 
Tuesday                  758 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.05 % 
Wednesday                779 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.41 % 
Thursday                 820 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.12 % 
Friday                   809 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Saturday                 900 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   923 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.89 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
YAML                     1 hr 47 mins        █████████░░░░░░░░░░░░░░░░   34.46 % 
Docker                   50 mins             ████░░░░░░░░░░░░░░░░░░░░░   16.20 % 
Bash                     44 mins             ████░░░░░░░░░░░░░░░░░░░░░   14.12 % 
Markdown                 37 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.99 % 
PHP                      34 mins             ███░░░░░░░░░░░░░░░░░░░░░░   11.03 % 

🔥 Editors: 
VS Code                  4 hrs 50 mins       ███████████████████████░░   93.00 % 
Obsidian                 21 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   07.00 % 

💻 Operating System: 
Linux                    5 hrs 12 mins       █████████████████████████   100.00 % 
```


 Last Updated on 30/08/2023 00:09:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
