---
marp: true
---

# Презентация из Markdown

Сделано с помощью пакета [marp](https://marp.app/).

---

# Компиляция:

Для компиляции слайдов в pdf можно либо поставить Nodejs и запускать Marp напрямую
```
npx @marp-team/marp-cli@latest slide-deck.md --allow-local-files  --pdf
```

Либо ничего не ставить и дёргать докер:
```
sudo docker run --rm --init -v $PWD:/home/marp/app/ -e LANG=$LANG -e MARP_USER="$(id -u):$(id -g)"  marpteam/marp-cli slide-deck.md  --allow-local-files  --pdf 
```
 