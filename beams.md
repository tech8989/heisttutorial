### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Beams of Color

## Step 1
壁にある色付きブロックと同じ色順になるように、色付きガラスを置こう。  
  
**ブロックの説明:**  
``||ww:動く [前] (0)歩||`` ワンダーウーマンを指定したブロック分 動かせる。  
``||ww:向きを変える [左]||`` ワンダーウーマンの向きを変える。  
``||ww:置く [黄色] ステンドグラス [前]||`` ワンダーウーマンにガラスを置かせる。  

#### ~ tutorialhint 
```blocks
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.RedStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.LimeStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.BlueStainedGlass, Direction.Left)
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.YellowStainedGlass, Direction.Left)
})

```
```ghost
player.onChat("run", function () {
    for (let index = 0; index < 4; index++) {
        ww.moveWW(Direction.Forward, 1)
        ww.turnWW(LEFT_TURN)
        ww.placeBlock(BeamsGlass.YellowStainedGlass, Direction.Forward)
    }
})
```
```template
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 3)
    ww.placeBlock(BeamsGlass.LimeStainedGlass, Direction.Right)
})
```


```package
minecraft-wwheist=github:tech8989/wwheist
```