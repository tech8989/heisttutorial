### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @flyoutOnly true
### @hideIteration true
### @explicitHints 1

# Hidden in Plain Sight

## Step 1
�Q���҂ɂ܂��ꂽ�D�_���݂��āA���܂��悤�B  
����ŁA�G�悪���ׂČ������B
  
�����͉��p�^�[��������̂ŁA�����ȃp�^�[�����l���Ă݂悤�B  
  
**�u���b�N�̐���:**  
``||ww:�Q���҂͓D�_��[�O]||`` �w�肵�������̎Q���҂��D�_�����ׂ���B  
``||ww:�D�_��߂܂��� [�O]||`` �w�肵�������̓D�_��߂܂���B

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