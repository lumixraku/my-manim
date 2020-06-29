
# requirements
docker and eulertour/manim

PS: eulertour/manim is too old for some examples.

You can build your own manim image from [manim](https://github.com/3b1b/manim)

# How to run

这里 `docker-compose run manim` 运行 compose 文件中的 manim service

compose 文件一个service 描述了一个容器

mymanim 使用的镜像是 mmm  mmm 是根据最新manim build 出的image

```
INPUT_PATH=~/repos/Others/my-manim \
OUTPUT_PATH=~/repos/Others/manimOutput \
docker-compose run manim matrix.py test -l


INPUT_PATH=~/repos/Others/my-manim \
OUTPUT_PATH=~/repos/Others/manimOutput \
docker-compose run mymanim fireworks.py scene -l


INPUT_PATH=~/repos/Others/my-manim \
OUTPUT_PATH=~/repos/Others/manimOutput \
docker-compose run mymanim matrix.py test -l

INPUT_PATH=~/repos/Others/my-manim \
OUTPUT_PATH=~/repos/Others/manimOutput \
docker-compose run mymanim say_i_love_u_by_math.py scene1 -l
```