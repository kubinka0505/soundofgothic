<p align="center"><a href="https://soundofgothic.pl/"><img src="https://cdn.discordapp.com/attachments/312993895887929355/792059157711814686/SoundOfGothic.svg" width=750></a></p>

<p align="center"><a href="https://www.python.org/downloads/release/python-375/"><img src="https://img.shields.io/badge/Python-3.7.5-brightgreen?style=for-the-badge&logoColor=white&link=https://www.python.org/&https://www.python.org/downloads/&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA8AAAAPCAMAAAAMCGV4AAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAABVlBMVEUAAAA5e7Q3ebA3eK43dak3dKY2dKI5gLg4ebA1eq83d6s3caI8aaU5e7M3eK42eKs4cJsAgIA4eK85d7A2dqs2dKk2dKc3cqR2koD/10v/20k2ebU4ebDRvlz/1UX/00Q4erDbxFf/0UA2eK42aZb/1ET/zz83d6s3cqQ6c6GZpXuprXCpq2y8s2P900X/00M3cKL/3lH/zDs2dKZVg5L/yjk3c6U3caJihoz/yTn/xzg7dp03bpuqqnH/0kP/0kD/0D7/zjz/yzz/wzz//wD/2E7/zj7/yDf/41X/1Ub/zj3/zTz/yjn/yDf/1Ub/00L/0ED/zj3/zDv/yTr/xzg3d6s3dak3dKc3cqQ3caI3cJ82bp03eK42bZr/10c2a5j/1UX/00P/0UE3dKb/zz//zT3/3U7/20z/2Ur/10j/1Ub/zj3/zDv/00T/0D//0kL/1ET///8twZG5AAAAVXRSTlMAVcbw67tCEuhD9/YRG/ukKQIgLYiIiL44MxUm3HX1QKxwwuqzlfj6/oVudnZvhf2fq/aydbYz7njbKQ0zLb13d3ciEQEaoSoJ7vxN4Rw3suj27MNWkzfuJAAAAAFiS0dEca8HXOIAAAAHdElNRQfkBQcLNhpsHcMTAAAAuklEQVQI12NgAAJGJuZQFlY2Bihg5+DkCguP4OaB8nn5+IHcyCgBME9QSFhEVEw8MipaQlKKgUFaJiYULBsdKxsnJ8+gAOfGKyYkKjEow7kqqolJagzqYckamlraOjq6evpJKakMLMkRBoZp6RmZWYlArhGDcUSkCYybnWPKYGYeZQHi5iblZedYWjEwWNvYArl29g6OTs4uYBe5AmXz89yM3KHu9fAsyM/z8vbxhXnIzz8gMCg4BMQEAKy7MbtksegJAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIwLTA1LTA3VDExOjU0OjI2KzAwOjAw1j8VsQAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMC0wNS0wN1QxMTo1NDoyNiswMDowMKdirQ0AAAAASUVORK5CYII="></a></p>

<p align="center"><a href="https://github.com/kubinka0505/soundofgothic/releases/"><img src="https://img.shields.io/github/v/release/kubinka0505/soundofgothic?style=for-the-badge"></a>　<a href="https://github.com/kubinka0505/soundofgothic/commit/"><img src="https://img.shields.io/github/last-commit/kubinka0505/soundofgothic?style=for-the-badge"></a></p>

<p align="center"><a href="https://github.com/kubinka0505/soundofgothic/issues/"><img src="https://img.shields.io/github/issues/kubinka0505/soundofgothic?style=for-the-badge"></a>　<a href="https://www.gnu.org/licenses/gpl-3.0.txt"><img src="https://img.shields.io/badge/license-GPL%20V3-red?style=for-the-badge"></a></p>

<p align="center"><img src="https://img.shields.io/codeclimate/maintainability/kubinka0505/soundofgothic?logo=code-climate&style=for-the-badge"></a></p>

## Description 📝
Simple Python API wrapper for [SoundOfGothic](https://soundofgothic.pl).


## Requirements 📥
- `Python >= 3.6`
- `requests >= 2.12.5`
---
## Installation 🖥️

1. `GitHub` Method **(recommended)**¹
	1. Clone the repository.
		```bash
		git clone https://github.com/kubinka0505/soundofgothic
		cd soundofgothic
		```
	2. Go to `Files` directory and install.
		```bash
		cd Files
		python setup.py install
		```
2. `pip` Method²
	1. Type into CMD: `python -m pip install soundofgothic`

¹ - Downloaded files are stored in `../soundofgothic/Files/soundofgothic/`

² - Downloaded files are stored in `../Lib/site-packages/soundofgothic/`

## Usage 📝

```python
>>> import soundofgothic as sog
>>>
>>> # Get dialog content
>>> Funny_Kharim = sog.Dialogs.search("powiedzmy sobie", version = 1)[0]
>>>
>>> Funny_Kharim["Content"]
'Powiedzmy sobie szczerze: przyszedłeś tutaj tylko dlatego, żeby móc pocałować Gomeza w dupę!'
>>>
>>> # Get dialogs containing "Kaffu" from Gothic 3
>>> Dialogs_List = sog.Dialogs.search("Kaffu", version = 3)
>>>
>>> # Find dialog URL from list by content
>>> URL = sog.Dialogs.Find.URL.by_content(Dialogs_List, "ulubieńców")
>>>
>>> # Download dialog file to given path
>>> sog.Dialogs.download(URL, r"C:\Users\Saturas\Desktop")
```

**[In case of problems create issue](https://github.com/kubinka0505/soundofgothic/issues/new/choose)**.
