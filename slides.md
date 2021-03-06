# Lets GO

---
# Co je GO
- Programovací Jazyk
- Striktně typovaný
- Kompilovaný
- GOLang
- Cčko na steroidech?
- Náhrada za python?

---
# Co je GO
![](images/griesemer-pike-thompson.png)
(Robert Griesemer, Rob Pike, Ken Thompson)

---
## Jaké je GO
# Mladé!

---
# Python - 1991
![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Macintosh_Portable-IMG_7541.jpg/2560px-Macintosh_Portable-IMG_7541.jpg)

---
# PHP - 1995
![](https://upload.wikimedia.org/wikipedia/commons/c/cc/Powerbook_190.jpg)

---
# C - 1972
![](https://pbs.twimg.com/media/EG_SoeKXkAEjaJR.jpg)

---
# GO - 2007
![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/Macbook_white_redjar_20060603.jpg/1920px-Macbook_white_redjar_20060603.jpg)

---
## Jaké je GO
# Minimalistické!

---
# Nemá objekty
![](https://live.staticflickr.com/7237/7404083572_6f51a14a74_b.jpg)

---
# Nemá dědičnost
![](https://media.giphy.com/media/l0HlKYxenTClHlOV2/source.gif)

---
# Nemá vyjímky
```
f, err := os.Open("filename.ext")
if err != nil {
   // Handle error
   log.Fatal(err)
}

// do something with the open *File f
```
---
# Nevyhneš se ukazatelům
![](https://imgs.xkcd.com/comics/pointers.png)

---
# GO má skvělý concurency pattern
![](https://media.giphy.com/media/l0HUln3LSwB1ym51u/source.gif)

---
# ... který běží na více jádrech
![](https://media.giphy.com/media/dZuvgnuNVohCarF0p4/giphy-downsized-large.gif)

---
# Příkaz GO
```
func main() {
   preheat_oven()
   go bake_meat()
   slice_the_salad()

   time.Sleep(time.Second) // Wait for meat
   plating()
}
```
---
# Je (jako) stavěný ma microservices
```
package main

import (
   "fmt",
   "net/http"
)

func hello(w http.ResponseWriter, req *http.Request) {
   fmt.Fprintf(w, "Heureka!")
}

func main() {
   http.HandleFunc("/", hello)
   http.ListenAndServe(":8090", nil)
}
```

---
# Vyrábí binárky
`
go build
`

---
# Vyrábí binárky
`
env GOOS=linux GOARCH=arm go build
`

---
# Spoustu věcí v základní knihovně
- HTTP server
- Testovací a benchmarkovací framework
- Crosscompile

---
# Go není python
![](https://www.eletimes.com/wp-content/uploads/2017/01/python_vs_golang-e1470416806915-300x196.jpg)

---
# Try GO
## https://play.golang.org/

---
![](https://media.giphy.com/media/zpVn8eb6NJnB6/source.gif)
