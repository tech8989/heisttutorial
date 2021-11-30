### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Dance Floor

## Step 1
ワンダーウーマンをプログラムして、壁にかかれているのと同じ色順で動くようにしよう。  
そうすれば、奥の壁にあるひみつのとびらが開くよ。

#### ~ tutorialhint 
```blocks
player.onChat("run", function () {
    ww.moveWW(Direction.Right, 4)
    ww.moveWW(Direction.Forward, 12)
    ww.moveWW(Direction.Right, 4)
})
player.onChat("run", function () {
    ww.turnWW(RIGHT_TURN)
    ww.moveWW(Direction.Forward, 4)
    ww.turnWW(LEFT_TURN)
    ww.moveWW(Direction.Forward, 12)
    ww.turnWW(RIGHT_TURN)
    ww.moveWW(Direction.Forward, 4)
})

```
```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    for (let index = 0; index < 4; index++) {
        
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(RIGHT_TURN)
})
```

```package
minecraft-wwheist=github:tech8989/wwheist
```