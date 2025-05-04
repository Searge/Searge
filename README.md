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
**I'm an Early 🐤** 

```text
🌞 Morning                1866 commits        ██████░░░░░░░░░░░░░░░░░░░   25.97 % 
🌆 Daytime                3027 commits        ███████████░░░░░░░░░░░░░░   42.14 % 
🌃 Evening                2034 commits        ███████░░░░░░░░░░░░░░░░░░   28.31 % 
🌙 Night                  257 commits         █░░░░░░░░░░░░░░░░░░░░░░░░   03.58 % 
```


📊 **This Week I Spent My Time On** 

```text
🕑︎ Time Zone: Europe/Kyiv

💬 Programming Languages: 
sh                       8 hrs 59 mins       █████████░░░░░░░░░░░░░░░░   34.89 % 
YAML                     4 hrs 36 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.89 % 
Terraform                4 hrs 34 mins       ████░░░░░░░░░░░░░░░░░░░░░   17.77 % 
JSON                     2 hrs 38 mins       ███░░░░░░░░░░░░░░░░░░░░░░   10.23 % 
Bash                     1 hr 48 mins        ██░░░░░░░░░░░░░░░░░░░░░░░   07.02 % 

🔥 Editors: 
VS Code                  16 hrs 6 mins       ████████████████░░░░░░░░░   62.52 % 
Zsh                      8 hrs 59 mins       █████████░░░░░░░░░░░░░░░░   34.89 % 
Obsidian                 25 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   01.64 % 
Sublime Text             13 mins             ░░░░░░░░░░░░░░░░░░░░░░░░░   00.87 % 
Vim                      1 min               ░░░░░░░░░░░░░░░░░░░░░░░░░   00.09 % 

💻 Operating System: 
Linux                    25 hrs 45 mins      █████████████████████████   100.00 % 
```


 Last Updated on 04/05/2025 00:07:34 UTC
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
