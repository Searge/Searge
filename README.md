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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C449%20hrs%2021%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1410 commits        ██████░░░░░░░░░░░░░░░░░░░   23.73 % 
🌆 Daytime                2636 commits        ███████████░░░░░░░░░░░░░░   44.36 % 
🌃 Evening                1659 commits        ███████░░░░░░░░░░░░░░░░░░   27.92 % 
🌙 Night                  237 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.99 % 
```
📅 **I'm Most Productive on Saturday** 

```text
Monday                   849 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.29 % 
Tuesday                  792 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.33 % 
Wednesday                805 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.55 % 
Thursday                 825 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.88 % 
Friday                   830 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.97 % 
Saturday                 921 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.50 % 
Sunday                   920 commits         ████░░░░░░░░░░░░░░░░░░░░░   15.48 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 43 mins             ███████████████░░░░░░░░░░   59.05 % 
YAML                     13 mins             ████░░░░░░░░░░░░░░░░░░░░░   17.98 % 
Bash                     6 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   08.91 % 
Nix                      5 mins              ██░░░░░░░░░░░░░░░░░░░░░░░   07.38 % 
Diff                     2 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   03.33 % 

🔥 Editors: 
Obsidian                 39 mins             █████████████░░░░░░░░░░░░   53.75 % 
VS Code                  30 mins             ██████████░░░░░░░░░░░░░░░   41.03 % 
Vim                      3 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   05.22 % 

💻 Operating System: 
Linux                    1 hr 13 mins        █████████████████████████   100.00 % 
```


 Last Updated on 08/04/2024 00:39:18 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
