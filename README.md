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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C449%20hrs%2034%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1414 commits        ██████░░░░░░░░░░░░░░░░░░░   23.78 % 
🌆 Daytime                2636 commits        ███████████░░░░░░░░░░░░░░   44.33 % 
🌃 Evening                1659 commits        ███████░░░░░░░░░░░░░░░░░░   27.90 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   853 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.35 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.32 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.54 % 
Thursday                 825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.87 % 
Friday                   830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.96 % 
Saturday                 921 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.49 % 
Sunday                   920 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.47 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 56 mins             ████████████████░░░░░░░░░   65.20 % 
YAML                     13 mins             ████░░░░░░░░░░░░░░░░░░░░░   15.18 % 
Bash                     6 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   07.62 % 
Nix                      5 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   06.30 % 
Diff                     2 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.84 % 

🔥 Editors: 
Obsidian                 53 mins             ███████████████░░░░░░░░░░   61.89 % 
VS Code                  28 mins             ████████░░░░░░░░░░░░░░░░░   33.65 % 
Vim                      3 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   04.46 % 

💻 Operating System: 
Linux                    1 hr 25 mins        █████████████████████████   100.00 % 
```


 Last Updated on 09/04/2024 00:40:55 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
