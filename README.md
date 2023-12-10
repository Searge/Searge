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
![Code Time](http://img.shields.io/badge/Code%20Time-2%2C349%20hrs%2048%20mins-blue)

**I'm an Early 🐤** 

```text
🌞 Morning                1527 commits        ██████░░░░░░░░░░░░░░░░░░░   22.56 % 
🌆 Daytime                3041 commits        ███████████░░░░░░░░░░░░░░   44.93 % 
🌃 Evening                1969 commits        ███████░░░░░░░░░░░░░░░░░░   29.09 % 
🌙 Night                  231 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.41 % 
```
📅 **I'm Most Productive on Sunday** 

```text
Monday                   995 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.70 % 
Tuesday                  873 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.90 % 
Wednesday                865 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.78 % 
Thursday                 943 commits         ███░░░░░░░░░░░░░░░░░░░░░░   13.93 % 
Friday                   858 commits         ███░░░░░░░░░░░░░░░░░░░░░░   12.68 % 
Saturday                 999 commits         ████░░░░░░░░░░░░░░░░░░░░░   14.76 % 
Sunday                   1235 commits        █████░░░░░░░░░░░░░░░░░░░░   18.25 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
Markdown                 2 hrs 32 mins       █████████████░░░░░░░░░░░░   50.04 % 
YAML                     56 mins             █████░░░░░░░░░░░░░░░░░░░░   18.69 % 
Other                    39 mins             ███░░░░░░░░░░░░░░░░░░░░░░   12.88 % 
SSH Config               19 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.40 % 
gitrebase                18 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   06.25 % 

🔥 Editors: 
VS Code                  2 hrs 38 mins       █████████████░░░░░░░░░░░░   52.27 % 
Obsidian                 1 hr 51 mins        █████████░░░░░░░░░░░░░░░░   36.68 % 
Vim                      25 mins             ██░░░░░░░░░░░░░░░░░░░░░░░   08.43 % 
Sublime Text             7 mins              █░░░░░░░░░░░░░░░░░░░░░░░░   02.62 % 

💻 Operating System: 
Linux                    5 hrs 3 mins        █████████████████████████   100.00 % 
```


 Last Updated on 10/12/2023 00:10:24 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
