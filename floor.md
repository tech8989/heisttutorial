### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Dance Floor

## Step 1
�����_�[�E�[�}�����v���O�������āA�ǂɂ�����Ă���̂Ɠ����F���œ����悤�ɂ��悤�B  
��������΁A���̕ǂɂ���Ђ݂̂Ƃт炪�J����B

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