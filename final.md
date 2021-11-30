### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Hidden in Plain Sight

## Step 1
参加者にまぎれた泥棒をみつけて、つかまえよう。  
これで、絵画がすべて見つかるよ。
  
答えは何パターンもあるので、いろんなパターンを考えてみよう。  
  
**ブロックの説明:**  
``||ww:参加者は泥棒か[前]||`` 指定した方向の参加者が泥棒か調べられる。  
``||ww:泥棒を捕まえる [前]||`` 指定した方向の泥棒を捕まえる。

```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    for (let index = 0; index < 4; index++) {
        
    }
    if (ww.locateGoon(Direction.Forward)) {
        ww.apprehendGoon(Direction.Forward)
    }
    while (!(false)) {
        
    }	
})
```
```template
player.onChat("run", function () {
    if (ww.locateGoon(Direction.Forward)) {

    }
})
```
```package
minecraft-wwheist=github:tech8989/wwheist
```