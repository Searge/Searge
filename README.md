## Hi 👋, I'm Searge

### An DevOps Engineer from Ukraine 🇺🇦

<a href="https://wakatime.com/@cdc825db-43f4-47e4-8c55-60641b31e257"><img src="https://wakatime.com/badge/user/cdc825db-43f4-47e4-8c55-60641b31e257.svg" alt="Total time coded since May 17 2018" /></a> <img src="https://komarev.com/ghpvc/?username=searge&label=Profile%20views&color=0e75b6&style=flat" alt="searge" /> [![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)

- 🌱 I’m currently learning **Full Stack Web Development**

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
    languages = ['Python', 'JS', 'HTML', 'CSS', 'XPath', 'Lisp']
    databases = ['SQLite', 'PostgreSQL', 'Percona', 'DynamoDB', 'Redis']
    misc = ['Linux', 'Shell', 'LXC', 'Docker', 'AWS']
    ongoing = ['Full Stack Web', 'Magento 2 Cloud', 'AWS']

    me = person('@Searge', 'Sergij Boremchuk',
                languages, databases, misc, ongoing)

    print(me.to_json())

# %%

```

<sub>Thanks @rednafi for idea of script :wink:</sub>

### My Stats

<!--START_SECTION:waka-->

<!--END_SECTION:waka-->

![footer](https://capsule-render.vercel.app/api?color=gradient&customColorList=14,21)
