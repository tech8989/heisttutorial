### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true 
### @explicitHints 1

# Suspicious Crates

## Step 1
たくさんの木箱の間を通って、ぬすまれた絵画の一部がないか調べよう。  
絵画があったら、その箱をこわして、手に入れよう。    
答えは何パターンもあるので、いろんなパターンを考えてみよう。    

**ブロックの説明:**  
``||ww:木箱の中に絵があるか調べる [前]||`` 指定した方向の木箱の中に、絵があるか調べられる。  
``||ww:木箱をこわす [前]||`` 指定した方向の木箱をこわす。絵があれば手に入る。

```ghost
player.onChat("run", function () {
    ww.moveWW(Direction.Forward, 1)
    ww.turnWW(LEFT_TURN)
    if (ww.locatePainting(Direction.Forward)) {
        ww.retrievePainting(Direction.Forward)
    }
    for (let index = 0; index < 4; index++) {
        
    }
    while (!(false)) {
        
    }	
})
```
```template
player.onChat("run", function () {
    if (ww.locatePainting(Direction.Forward)) {

    }
})
```
```package
minecraft-wwheist=github:tech8989/wwheist
```