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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C449%20hrs%202%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1407 commits        ██████░░░░░░░░░░░░░░░░░░░   23.71 % 
🌆 Daytime                2636 commits        ███████████░░░░░░░░░░░░░░   44.42 % 
🌃 Evening                1658 commits        ███████░░░░░░░░░░░░░░░░░░   27.94 % 
🌙 Night                  233 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.93 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   845 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.24 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.35 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.57 % 
Thursday                 825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.90 % 
Friday                   830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.99 % 
Saturday                 921 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.52 % 
Sunday                   916 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.44 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 29 mins             ████████████░░░░░░░░░░░░░   49.84 % 
YAML                     13 mins             ██████░░░░░░░░░░░░░░░░░░░   22.07 % 
Bash                     6 mins              ███░░░░░░░░░░░░░░░░░░░░░░   10.94 % 
Nix                      5 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   09.06 % 
Diff                     2 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   04.09 % 

🔥 Editors: 
VS Code                  30 mins             █████████████░░░░░░░░░░░░   50.37 % 
Obsidian                 25 mins             ███████████░░░░░░░░░░░░░░   43.33 % 
Vim                      3 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   06.29 % 

💻 Operating System: 
Linux                    59 mins             █████████████████████████   100.00 % 
```


 Last Updated on 07/04/2024 00:36:57 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
