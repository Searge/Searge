# Hi <img src="img/vulcan.webp" style="display: inline-block; margin: 0; height: 2rem" alt="Vulcan salute" />, I'm Searge

## An DevOps Engineer from Ukraine 🇺🇦

![Lutsk](img/flag_of_luts_k_by_ashikcygan_d62gwi3.png) ![Volyn](img/volyn_by_ashikcygan_d61v3xl.png) ![Ukraine](img/ukraine_by_stamps_of_flags_dbe6fld.png)

![Visitors](https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat) [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)

```python
"""Creating a class for keeping track of knowledge."""
import json
from rich import print
from dataclasses import asdict, make_dataclass

person = make_dataclass('Person',
                        [('nick', str),
                         ('name', str),
                            ('languages', list[str]),
                            ('databases', list[str]),
                            ('misc', list[str]),
                            ('ongoing', list[str])],
                        namespace={
                            'to_json': lambda self: json.dumps(
                                asdict(self), indent=4)})
# %%

if __name__ == '__main__':
    languages = ['YAML', 'Bash', 'Python', 'JS']
    databases = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc = ['Ci/Cd', 'Linux', 'Shell', 'LXC', 'Docker', 'Terraform', 'AWS']
    ongoing = ['Full Stack Web', 'Magento 2 Cloud', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```

<sub>Thanks @rednafi for idea of script :wink:</sub>

<!--START_SECTION:waka-->
<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=14,21&height=82&section=footer)
