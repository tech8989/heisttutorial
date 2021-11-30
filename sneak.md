### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Stealth Mission

## Step 1
アラームがならないようにレーザーをさけて、犯人の後ろに行けるように、  
ワンダーウーマンを動かそう。  
後ろについたら、``||ww:犯人を倒す [前]||`` を使って、犯人を倒そう。
  
**ブロックの説明:**  
``||ww:犯人を倒す [前]||`` 指定した方向の犯人を倒す。

#### ~ tutorialhint 
```blocks
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    ww.moveWW(Direction.Forward, 3)
    ww.turnWW(RIGHT_TURN)
    ww.moveWW(Direction.Forward, 6)
    ww.turnWW(RIGHT_TURN)
    ww.moveWW(Direction.Forward, 6)
    ww.turnWW(LEFT_TURN)
    ww.moveWW(Direction.Forward, 3)
    ww.turnWW(LEFT_TURN)
    ww.moveWW(Direction.Forward, 3)
    ww.turnWW(RIGHT_TURN)
    ww.moveWW(Direction.Forward, 2)
    ww.takedownGoon(Direction.Forward)
})
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.moveWW(Direction.Left, 3)
    ww.moveWW(Direction.Forward, 6)
    ww.moveWW(Direction.Right, 6)
    ww.moveWW(Direction.Forward, 3)
    ww.moveWW(Direction.Left, 3)
    ww.moveWW(Direction.Forward, 2)
    ww.takedownGoon(Direction.Forward)
})
```

```ghost
player.onChat("run", function () {
    for (let index = 0; index < 4; index++) {
        ww.moveWW(Direction.Forward, 1)
        ww.turnWW(LEFT_TURN)
        ww.takedownGoon(Direction.Forward)
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
})
```

```package
minecraft-wwheist=github:tech8989/wwheist
```